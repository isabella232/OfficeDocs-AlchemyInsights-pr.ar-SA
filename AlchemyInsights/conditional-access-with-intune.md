---
title: الوصول المشروط باستخدام Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704773"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="76973-102">الوصول المشروط باستخدام Intune</span><span class="sxs-lookup"><span data-stu-id="76973-102">Conditional Access with Intune</span></span>

<span data-ttu-id="76973-103">يتطلب  **استخدام "الوصول المشروط"**  مع Intune ثلاث خطوات:</span><span class="sxs-lookup"><span data-stu-id="76973-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="76973-104">قم بإنشاء  **نهج توافق**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android)أو  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios)أو  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)لتحديد الإعدادات التي يجب أن يتم التحقق من مطابقتها قبل أن يعتبر الجهاز متوافقا.</span><span class="sxs-lookup"><span data-stu-id="76973-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="76973-105">على سبيل المثال، يجب أن يكون رقم pin في الجهاز 6 أرقام على الأقل قبل أن يعتبر متوافقا.</span><span class="sxs-lookup"><span data-stu-id="76973-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="76973-106">أنشئ نهج **الوصول المشروط**  الذي يحدد الموارد التي يتم حمايتها، والشروط التي يجب أن يتم تأمينها للوصول إلى تلك الموارد.</span><span class="sxs-lookup"><span data-stu-id="76973-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="76973-107">[على سبيل المثال،](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  يجب أن يكون الجهاز متوافقا قبل الوصول إلى البريد الإلكتروني الخاص بالشركة.</span><span class="sxs-lookup"><span data-stu-id="76973-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="76973-108">تأكد من **أن كل**  من "سياسات التوافق" و"سياسات  **الوصول**  المشروط" تستهدف مجموعات المستخدمين المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="76973-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="76973-109">قد يتطلب ذلك إنشاء مجموعات معينة من المستخدمين في Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="76973-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="76973-110">**ارتباطات مفيدة:**</span><span class="sxs-lookup"><span data-stu-id="76973-110">**Helpful links:**</span></span>

[<span data-ttu-id="76973-111">نظرة عامة حول توافق الجهاز</span><span class="sxs-lookup"><span data-stu-id="76973-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="76973-112">استكشاف الأخطاء الم CA وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="76973-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="76973-113">نهج استكشاف الأخطاء وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="76973-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="76973-114">لحماية البريد الإلكتروني (Exchange Online) من الوصول بواسطة الأجهزة غير المتوافقة، يجب أن يكون المستندان متبوعين بما يلي:</span><span class="sxs-lookup"><span data-stu-id="76973-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="76973-115">حماية الوصول إلى البريد الإلكتروني من الأجهزة التي تستخدم EAS</span><span class="sxs-lookup"><span data-stu-id="76973-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="76973-116">حماية الوصول إلى البريد الإلكتروني من الأجهزة التي تستخدم عملاء المصادقة الحديثة مثل Outlook</span><span class="sxs-lookup"><span data-stu-id="76973-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)