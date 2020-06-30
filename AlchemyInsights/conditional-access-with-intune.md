---
title: الوصول المشروط مع Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931402"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="9b554-102">الوصول المشروط مع Intune</span><span class="sxs-lookup"><span data-stu-id="9b554-102">Conditional Access with Intune</span></span>

<span data-ttu-id="9b554-103">استخدام **"الوصول المشروط"** مع Intune يتطلب 3 خطوات:</span><span class="sxs-lookup"><span data-stu-id="9b554-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="9b554-104">إنشاء **سياسة التوافق** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) لتحديد الإعدادات التي يجب تلبيتها قبل اعتبار الجهاز متوافقًا.</span><span class="sxs-lookup"><span data-stu-id="9b554-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="9b554-105">على سبيل المثال، يجب أن يكون الجهاز دبوس من 6 أرقام على الأقل قبل أن يعتبر متوافقاً.</span><span class="sxs-lookup"><span data-stu-id="9b554-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="9b554-106">إنشاء **نهج الوصول المشروط** الذي يحدد ما هي الموارد التي يتم حماية و الشروط التي يجب تلبيتها للوصول إلى تلك الموارد.</span><span class="sxs-lookup"><span data-stu-id="9b554-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="9b554-107">[على سبيل المثال،](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) يجب أن يكون الجهاز متوافقًا قبل الوصول إلى البريد الإلكتروني للشركة.</span><span class="sxs-lookup"><span data-stu-id="9b554-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="9b554-108">تأكد من أن كلاً من **سياسات التوافق** وسياسات **الوصول المشروط** تستهدف مجموعات المستخدمين المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="9b554-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="9b554-109">قد يتطلب ذلك إنشاء مجموعات معينة من المستخدمين في "خدمة Active Directory Azure".</span><span class="sxs-lookup"><span data-stu-id="9b554-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="9b554-110">**روابط مفيدة:**</span><span class="sxs-lookup"><span data-stu-id="9b554-110">**Helpful links:**</span></span>

[<span data-ttu-id="9b554-111">نظرة عامة حول توافق الجهاز</span><span class="sxs-lookup"><span data-stu-id="9b554-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="9b554-112">CA استكشاف الأخطاء وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="9b554-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="9b554-113">نهج استكشاف الأخطاء وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="9b554-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="9b554-114">لحماية البريد الإلكتروني (Exchange عبر الإنترنت) من الوصول من قبل الأجهزة غير المتوافقة، يجب اتباع كلا المستندين:</span><span class="sxs-lookup"><span data-stu-id="9b554-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="9b554-115">حماية الوصول إلى البريد الإلكتروني من الأجهزة التي تستخدم EAS</span><span class="sxs-lookup"><span data-stu-id="9b554-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="9b554-116">حماية الوصول إلى البريد الإلكتروني من الأجهزة التي تستخدم عملاء المصادقة الحديثة مثل Outlook</span><span class="sxs-lookup"><span data-stu-id="9b554-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)