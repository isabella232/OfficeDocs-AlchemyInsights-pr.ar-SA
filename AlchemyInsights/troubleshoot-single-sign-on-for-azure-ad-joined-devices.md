---
title: استكشاف الأخطاء في تسجيل الدخول المفرد للأجهزة المنضمة إلى Azure AD وإصلاحها
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034799"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="ee1cb-102">استكشاف الأخطاء في تسجيل الدخول المفرد للأجهزة المنضمة إلى Azure AD وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="ee1cb-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="ee1cb-103">إذا كانت لديك بيئة Active Directory (AD) المحلية وتريد الانضمام إلى أجهزة الكمبيوتر المنضمة إلى مجال AD إلى Azure AD، يمكنك تنفيذ ذلك من خلال القيام بضم Azure AD المختلط.</span><span class="sxs-lookup"><span data-stu-id="ee1cb-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="ee1cb-104">كيفية: يوفر لك تنفيذ الانضمام إلى [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) المختلط الخطوات ذات الصلة لتنفيذ صلة Azure AD مختلطة في بيئتك.</span><span class="sxs-lookup"><span data-stu-id="ee1cb-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="ee1cb-105">لمزيد من المعلومات، راجع تكوين الأجهزة المنضمة إلى [Azure AD](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)ل Windows AD Single-Sign تشغيل باستخدام Windows Hello for Business .</span><span class="sxs-lookup"><span data-stu-id="ee1cb-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="ee1cb-106">**مشاكل رمز التحديث المميز الأساسي (PRT)**</span><span class="sxs-lookup"><span data-stu-id="ee1cb-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="ee1cb-107">رمز التحديث المميز الأساسي (PRT) هو الأداة الرئيسية لمصادقة Azure AD على أجهزة Windows 10 و Windows Server 2016 والإصدارات الأحدث و iOS و Android.</span><span class="sxs-lookup"><span data-stu-id="ee1cb-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="ee1cb-108">إنه رمز JSON Web Token (JWT) تم إصداره خصيصا ل وسيطي الرمز المميز من جهة Microsoft الأولى لتمكين تسجيل الدخول الفردي (SSO) عبر التطبيقات المستخدمة على هذه الأجهزة.</span><span class="sxs-lookup"><span data-stu-id="ee1cb-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="ee1cb-109">للحصول على تفاصيل حول كيفية إصدار PRT، استخدامه، وحمايته على أجهزة Windows 10، راجع [ما هو رمز التحديث المميز الأساسي؟](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="ee1cb-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="ee1cb-110">**WamDefaultSet: YES و AzureADPrt: YES**</span><span class="sxs-lookup"><span data-stu-id="ee1cb-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="ee1cb-111">تشير هذه الحقول إلى ما إذا كان المستخدم قد مصادقة على Azure AD بنجاح عند تسجيل الدخول إلى الجهاز.</span><span class="sxs-lookup"><span data-stu-id="ee1cb-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="ee1cb-112">إذا كانت القيم **لا**، فقد يكون ذلك بسبب:</span><span class="sxs-lookup"><span data-stu-id="ee1cb-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="ee1cb-113">مفتاح تخزين غير صحيح في TPM المقترن بجهاز عند التسجيل (تحقق من KeySignTest أثناء التشغيل غير المرتد)</span><span class="sxs-lookup"><span data-stu-id="ee1cb-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="ee1cb-114">"معرّف تسجيل الدخول البديل"</span><span class="sxs-lookup"><span data-stu-id="ee1cb-114">Alternate Login ID</span></span>
- <span data-ttu-id="ee1cb-115">لم يتم العثور على وكيل HTTP</span><span class="sxs-lookup"><span data-stu-id="ee1cb-115">HTTP Proxy not found</span></span>

<span data-ttu-id="ee1cb-116">لا استكشاف الأخطاء وإصلاحها في الأجهزة باستخدام الأمر dsregcmd، راجع [حالة SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="ee1cb-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
