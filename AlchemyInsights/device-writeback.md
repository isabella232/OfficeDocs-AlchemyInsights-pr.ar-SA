---
title: Device Writeback
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256659"
---
# <a name="device-writeback"></a><span data-ttu-id="28294-102">Device Writeback</span><span class="sxs-lookup"><span data-stu-id="28294-102">Device Writeback</span></span>

<span data-ttu-id="28294-103">يتم استخدام Device Writeback في السيناريوهات التالية:</span><span class="sxs-lookup"><span data-stu-id="28294-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="28294-104">تمكين [Windows Hello for Business باستخدام نشر الثقة بالشهادات المختلطة](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span><span class="sxs-lookup"><span data-stu-id="28294-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="28294-105">تمكين الوصول الشرطي استنادا إلى الأجهزة التي تم توفيرها للتطبيقات المحمية من ADFS (2012 R2 أو أعلى) (ثقة الطرف المعتمد)</span><span class="sxs-lookup"><span data-stu-id="28294-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="28294-106">الاشتراك في Azure AD Premium مطلوب لكتابه الجهاز.</span><span class="sxs-lookup"><span data-stu-id="28294-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="28294-107">ويوفر ذلك المزيد من الأمان وضمانة أن الوصول إلى التطبيقات يتم منحه للأجهزة الموثوق بها فقط.</span><span class="sxs-lookup"><span data-stu-id="28294-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="28294-108">للحصول على مزيد من [](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) المعلومات حول "الوصول الشرطي"، راجع "إدارة المخاطر" باستخدام "الوصول المشروط" وإعداد "الوصول المشروط" في الموقع باستخدام تسجيل جهاز [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/devices/overview)</span><span class="sxs-lookup"><span data-stu-id="28294-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="28294-109">لمزيد من المعلومات حول تمكين "إعادة كتابة الجهاز" للأجهزة، راجع ["تمكين كتابة الجهاز".](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)</span><span class="sxs-lookup"><span data-stu-id="28294-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
