---
title: مراقبة الوصول المشروط
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28274017"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="bf794-102">مراقبة الوصول المشروط</span><span class="sxs-lookup"><span data-stu-id="bf794-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="bf794-p101">سيتلقى المستخدمون المستهدفة مع الوصول المشروط إعلام بالبريد إلكتروني إذا لم تتوافق مع متطلبات الوصول الخاصة بمؤسستك. لحل ذلك، نوصي واحداً أو أكثر من الحلول التالية:</span><span class="sxs-lookup"><span data-stu-id="bf794-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="bf794-p102">إذا كان الجهاز الذي يفترض فيه أن تسجيلهم، المشورة للمستخدم بالانتقال إلى تطبيق "مدخل الشركة" والتحقق من أنها تظهر في "مدخل الشركة على الإنترنت". إذا لم يحدث ذلك، يجب على المستخدم تسجيل الجهاز.</span><span class="sxs-lookup"><span data-stu-id="bf794-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="bf794-p103">الانتقال إلى موقع Azure **إينتوني \> توافق الجهاز**. تحت **مراقبة** انقر فوق **توافق الأجهزة**. عرض تقرير توافق الجهاز الخاص بك للتحقق من أن الجهاز الخاص بالمستخدم يتم وضع علامة متوافق كما.</span><span class="sxs-lookup"><span data-stu-id="bf794-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="bf794-p104">الانتقال إلى موقع Azure **إينتوني \> توافق الجهاز**. ضمن **إدارة**، انقر فوق **نهج**. في قائمة نهج التوافق، تحقق من أنه تم تعيين تشكيل جانبي للجهاز المستخدم. إذا تم تعيين أي ملف تعريف، ثم إينتوني لن قادرة على تأكيد حالة الامتثال للجهاز.</span><span class="sxs-lookup"><span data-stu-id="bf794-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="bf794-114">تحرير تعيين الوصول الشرطي الخاص بالمستخدم.</span><span class="sxs-lookup"><span data-stu-id="bf794-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="bf794-115">الانتقال إلى موقع Azure **إينتوني \> الوصول الشرطي \> نهج**</span><span class="sxs-lookup"><span data-stu-id="bf794-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="bf794-116">حدد نهج من القائمة</span><span class="sxs-lookup"><span data-stu-id="bf794-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="bf794-117">انقر فوق **المستخدمين والمجموعات**</span><span class="sxs-lookup"><span data-stu-id="bf794-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="bf794-p105">لاستهداف سياسة معينة على شخص ما، عليك إضافتها إلى قائمة **التضمين** . للتأكد من حذف شخص من النهج، إضافتها إلى قائمة **استبعاد** .</span><span class="sxs-lookup"><span data-stu-id="bf794-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="bf794-120">اقرأ المزيد: [كيفية "مراقبة الوصول المشروط" الأجهزة](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="bf794-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

