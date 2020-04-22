---
title: مراقبة الوصول المشروط
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713705"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="87568-102">مراقبة الوصول المشروط للتبادل</span><span class="sxs-lookup"><span data-stu-id="87568-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="87568-103">سيتلقى المستخدمون المستهدفون بالوصول المشروط رسالة إعلام إلكترونية إذا لم يستوفوا متطلبات الوصول الخاصة بمؤسستك.</span><span class="sxs-lookup"><span data-stu-id="87568-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="87568-104">لحل، نوصي واحد أو أكثر من الحلول التالية:</span><span class="sxs-lookup"><span data-stu-id="87568-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="87568-105">إذا كان من المفترض أن يكون الجهاز مسجلًا، فنصح المستخدم بالذهاب إلى تطبيق بوابة الشركة والتحقق من ظهوره في بوابة الشركة.</span><span class="sxs-lookup"><span data-stu-id="87568-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="87568-106">إذا لم يكن كذلك، يجب على المستخدم تسجيل الجهاز.</span><span class="sxs-lookup"><span data-stu-id="87568-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="87568-107">في بوابة Azure انتقل إلى \*\*توافق الجهاز Intune \> \*\*.</span><span class="sxs-lookup"><span data-stu-id="87568-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="87568-108">ضمن **مراقبة** انقر فوق **التوافق الجهاز**.</span><span class="sxs-lookup"><span data-stu-id="87568-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="87568-109">عرض تقرير امتثال جهازك للتحقق من أن جهاز المستخدم متوافق.</span><span class="sxs-lookup"><span data-stu-id="87568-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="87568-110">في بوابة Azure انتقل إلى \*\*توافق الجهاز Intune \> \*\*.</span><span class="sxs-lookup"><span data-stu-id="87568-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="87568-111">ضمن **إدارة،** انقر فوق **النُهج**.</span><span class="sxs-lookup"><span data-stu-id="87568-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="87568-112">في قائمة نُهج التوافق، تحقق من تعيين ملف تعريف إلى جهاز المستخدم.</span><span class="sxs-lookup"><span data-stu-id="87568-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="87568-113">إذا لم يتم تعيين ملف تعريف، فلن يتمكن Intune من تأكيد حالة توافق الجهاز.</span><span class="sxs-lookup"><span data-stu-id="87568-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="87568-114">تحرير تعيين الوصول الشرطي للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="87568-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="87568-115">في بوابة Azure انتقل إلى **سياسات الوصول \> \> المشروط Intune**</span><span class="sxs-lookup"><span data-stu-id="87568-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="87568-116">تحديد نهج من القائمة</span><span class="sxs-lookup"><span data-stu-id="87568-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="87568-117">انقر على **المستخدمين والمجموعات**</span><span class="sxs-lookup"><span data-stu-id="87568-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="87568-118">لاستهداف نهج معين تجاه شخص ما، قم بإضافته إلى قائمة **تضمين.**</span><span class="sxs-lookup"><span data-stu-id="87568-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="87568-119">للتأكد من حذف شخص من النهج، قم بإضافته إلى قائمة **الاستبعاد.**</span><span class="sxs-lookup"><span data-stu-id="87568-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="87568-120">اقرأ المزيد: [كيفية مراقبة أجهزة الوصول المشروط](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="87568-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

