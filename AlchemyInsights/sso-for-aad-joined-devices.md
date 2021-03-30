---
title: Single-Sign على الأجهزة المنضمة إلى Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404185"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="64a09-102">تسجيل الدخول المفرد للأجهزة المنضمة إلى Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="64a09-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="64a09-103">إذا كانت لديك بيئة Active Directory (AD) المحلية وتريد الانضمام إلى أجهزة الكمبيوتر المنضمة إلى مجال AD إلى Azure AD، يمكنك تنفيذ ذلك من خلال القيام بضم Azure AD المختلط.</span><span class="sxs-lookup"><span data-stu-id="64a09-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="64a09-104">كيفية: يوفر لك تنفيذ الانضمام إلى [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) المختلط الخطوات ذات الصلة لتنفيذ صلة Azure AD مختلطة في بيئتك.</span><span class="sxs-lookup"><span data-stu-id="64a09-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="64a09-105">تكوين أجهزة Azure AD المتصلة بأجهزة التشغيل Single-Sign باستخدام Windows Hello for Business</span><span class="sxs-lookup"><span data-stu-id="64a09-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="64a09-106">**مشاكل رمز التحديث المميز الأساسي (PRT)** رمز التحديث المميز الأساسي (PRT) هو الأداة الرئيسية لمصادقة Azure AD على أجهزة Windows 10 و Windows Server 2016 والإصدارات الأحدث و iOS و Android.</span><span class="sxs-lookup"><span data-stu-id="64a09-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="64a09-107">إنه رمز JSON Web Token (JWT) تم إصداره خصيصا ل وسيطي الرمز المميز من جهة Microsoft الأولى لتمكين تسجيل الدخول الفردي (SSO) عبر التطبيقات المستخدمة على هذه الأجهزة.</span><span class="sxs-lookup"><span data-stu-id="64a09-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="64a09-108">[في ما هو](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)رمز التحديث المميز الأساسي؟ ، سنوفر تفاصيل حول كيفية إصدار PRT، استخدامه، وحمايته على أجهزة Windows 10.</span><span class="sxs-lookup"><span data-stu-id="64a09-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="64a09-109">**WamDefaultSet: YES و AzureADPrt: YES** تشير هذه الحقول إلى ما إذا كان المستخدم قد مصادقة على Azure AD بنجاح عند تسجيل الدخول إلى الجهاز.</span><span class="sxs-lookup"><span data-stu-id="64a09-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="64a09-110">إذا كانت القيم **NO**، فقد تكون مستحقة:</span><span class="sxs-lookup"><span data-stu-id="64a09-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="64a09-111">مفتاح تخزين غير صحيح في TPM المقترن بجهاز عند التسجيل (تحقق من KeySignTest أثناء التشغيل غير المرتد).</span><span class="sxs-lookup"><span data-stu-id="64a09-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="64a09-112">"معرّف تسجيل الدخول البديل"</span><span class="sxs-lookup"><span data-stu-id="64a09-112">Alternate Login ID</span></span>
- <span data-ttu-id="64a09-113">لم يتم العثور على وكيل HTTP</span><span class="sxs-lookup"><span data-stu-id="64a09-113">HTTP Proxy not found</span></span>

<span data-ttu-id="64a09-114">استكشاف الأخطاء وإصلاحها باستخدام الأمر dsregcmd - [حالة SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="64a09-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
