---
title: مراقبة الوصول المشروط
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418456"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="0f1b0-102">مراقبة الوصول المشروط</span><span class="sxs-lookup"><span data-stu-id="0f1b0-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="0f1b0-103">سيتلقى المستخدمون المستهدفة مع الوصول المشروط إعلام بالبريد إلكتروني إذا لم تتوافق مع متطلبات الوصول الخاصة بمؤسستك.</span><span class="sxs-lookup"><span data-stu-id="0f1b0-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="0f1b0-104">لحل ذلك، نوصي واحداً أو أكثر من الحلول التالية:</span><span class="sxs-lookup"><span data-stu-id="0f1b0-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="0f1b0-105">إذا كان الجهاز الذي يفترض فيه أن تسجيلهم، المشورة للمستخدم بالانتقال إلى تطبيق "مدخل الشركة" والتحقق من أنها تظهر في "مدخل الشركة على الإنترنت".</span><span class="sxs-lookup"><span data-stu-id="0f1b0-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="0f1b0-106">إذا لم يحدث ذلك، يجب على المستخدم تسجيل الجهاز.</span><span class="sxs-lookup"><span data-stu-id="0f1b0-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="0f1b0-107">الانتقال إلى موقع Azure **إينتوني \> توافق الجهاز**.</span><span class="sxs-lookup"><span data-stu-id="0f1b0-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="0f1b0-108">تحت **مراقبة** انقر فوق **توافق الأجهزة**.</span><span class="sxs-lookup"><span data-stu-id="0f1b0-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="0f1b0-109">عرض تقرير توافق الجهاز الخاص بك للتحقق من أن الجهاز الخاص بالمستخدم يتم وضع علامة متوافق كما.</span><span class="sxs-lookup"><span data-stu-id="0f1b0-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="0f1b0-110">الانتقال إلى موقع Azure **إينتوني \> توافق الجهاز**.</span><span class="sxs-lookup"><span data-stu-id="0f1b0-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="0f1b0-111">ضمن **إدارة**، انقر فوق **نهج**.</span><span class="sxs-lookup"><span data-stu-id="0f1b0-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="0f1b0-112">في قائمة نهج التوافق، تحقق من أنه تم تعيين تشكيل جانبي للجهاز المستخدم.</span><span class="sxs-lookup"><span data-stu-id="0f1b0-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="0f1b0-113">إذا تم تعيين أي ملف تعريف، ثم إينتوني لن قادرة على تأكيد حالة الامتثال للجهاز.</span><span class="sxs-lookup"><span data-stu-id="0f1b0-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="0f1b0-114">تحرير تعيين الوصول الشرطي الخاص بالمستخدم.</span><span class="sxs-lookup"><span data-stu-id="0f1b0-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="0f1b0-115">الانتقال إلى موقع Azure **إينتوني \> الوصول الشرطي \> نهج**</span><span class="sxs-lookup"><span data-stu-id="0f1b0-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="0f1b0-116">حدد نهج من القائمة</span><span class="sxs-lookup"><span data-stu-id="0f1b0-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="0f1b0-117">انقر فوق **المستخدمين والمجموعات**</span><span class="sxs-lookup"><span data-stu-id="0f1b0-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="0f1b0-118">لاستهداف سياسة معينة على شخص ما، عليك إضافتها إلى قائمة **التضمين** .</span><span class="sxs-lookup"><span data-stu-id="0f1b0-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="0f1b0-119">للتأكد من حذف شخص من النهج، إضافتها إلى قائمة **استبعاد** .</span><span class="sxs-lookup"><span data-stu-id="0f1b0-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="0f1b0-120">اقرأ المزيد: [كيفية "مراقبة الوصول المشروط" الأجهزة](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="0f1b0-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

