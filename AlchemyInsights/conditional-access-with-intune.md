---
title: وصول شرطي باستخدام Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807646"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="085cf-102">وصول شرطي باستخدام Intune</span><span class="sxs-lookup"><span data-stu-id="085cf-102">Conditional Access with Intune</span></span>

<span data-ttu-id="085cf-103">يتطلب استخدام  **Access الشرطي**  مع Intune وجود 3 خطوات:</span><span class="sxs-lookup"><span data-stu-id="085cf-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="085cf-104">أنشئ  **نهج توافق**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android)،  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios)،  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) لتحديد الإعدادات التي يجب استيفاءها قبل ان يتم اعتبار الجهاز متوافقا.</span><span class="sxs-lookup"><span data-stu-id="085cf-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="085cf-105">علي سبيل المثال ، يجب ان يتوفر للجهاز رقم pin يتكون من 6 أرقام علي الأقل قبل ان يتم اعتباره متوافقا.</span><span class="sxs-lookup"><span data-stu-id="085cf-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="085cf-106">قم بإنشاء **نهج وصول شرطي**  يحدد الموارد التي يتم حمايتها ، والشروط التي يجب استيفاءها للوصول إلى هذه الموارد.</span><span class="sxs-lookup"><span data-stu-id="085cf-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="085cf-107">[علي سبيل المثال ،](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  يجب ان يكون الجهاز متوافقا قبل الوصول إلى البريد الكتروني للشركة.</span><span class="sxs-lookup"><span data-stu-id="085cf-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="085cf-108">تاكد من استهداف كل من **نهج التوافق**  **ونهج الوصول الشرطي**  لمجموعات المستخدمين المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="085cf-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="085cf-109">قد يتطلب ذلك إنشاء مجموعات معينه من المستخدمين في Azure Active directory.</span><span class="sxs-lookup"><span data-stu-id="085cf-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="085cf-110">**الارتباطات المفيدة:**</span><span class="sxs-lookup"><span data-stu-id="085cf-110">**Helpful links:**</span></span>

[<span data-ttu-id="085cf-111">نظره عامه علي توافق الاجهزه</span><span class="sxs-lookup"><span data-stu-id="085cf-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="085cf-112">استكشاف أخطاء المراجع المصدقة</span><span class="sxs-lookup"><span data-stu-id="085cf-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="085cf-113">نهج استكشاف الأخطاء وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="085cf-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="085cf-114">لحماية البريد الكتروني (Exchange online) من access بواسطة الاجهزه غير المتوافقة ، يجب اتباع كلا المستندين:</span><span class="sxs-lookup"><span data-stu-id="085cf-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="085cf-115">حماية الوصول إلى البريد الكتروني من الاجهزه باستخدام EAS</span><span class="sxs-lookup"><span data-stu-id="085cf-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="085cf-116">حماية الوصول إلى البريد الكتروني من الاجهزه باستخدام عملاء المصادقة الحديثة مثل Outlook</span><span class="sxs-lookup"><span data-stu-id="085cf-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)