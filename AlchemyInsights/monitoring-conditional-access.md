---
title: مراقبه الوصول الشرطي
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702890"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="807f9-102">مراقبه الوصول الشرطي ل Exchange</span><span class="sxs-lookup"><span data-stu-id="807f9-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="807f9-103">سيتلقى المستخدمون الذين يستهدفون access الشرطي بريدا الكترونيا للاعلام إذا لم يستوفوا متطلبات الوصول الخاصة بمؤسسك.</span><span class="sxs-lookup"><span data-stu-id="807f9-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="807f9-104">لحل هذه المشكلة ، نوصي باجراء واحد أو أكثر من الحلول التالية:</span><span class="sxs-lookup"><span data-stu-id="807f9-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="807f9-105">إذا كان الجهاز بريسوميد بالتسجيل ، فيمكنك اشعار المستخدم بالانتقال إلى تطبيق مدخل الشركة والتحقق من انه يظهر في مدخل الشركة.</span><span class="sxs-lookup"><span data-stu-id="807f9-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="807f9-106">إذا لم يكن كذلك ، فيجب علي المستخدم تسجيل الجهاز.</span><span class="sxs-lookup"><span data-stu-id="807f9-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="807f9-107">في مدخل Azure ، انتقل إلى \*\* \> توافق الجهاز في Intune\*\*.</span><span class="sxs-lookup"><span data-stu-id="807f9-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="807f9-108">ضمن **جهاز العرض** ، انقر فوق **توافق الجهاز**.</span><span class="sxs-lookup"><span data-stu-id="807f9-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="807f9-109">اعرض تقرير توافق الاجهزه للتحقق من انه تم وضع علامة علي جهاز المستخدم علي انه متوافق.</span><span class="sxs-lookup"><span data-stu-id="807f9-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="807f9-110">في مدخل Azure ، انتقل إلى \*\* \> توافق الجهاز في Intune\*\*.</span><span class="sxs-lookup"><span data-stu-id="807f9-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="807f9-111">ضمن **أداره**، انقر فوق **النهج**.</span><span class="sxs-lookup"><span data-stu-id="807f9-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="807f9-112">في قائمه نهج التوافق ، تحقق من انه تم تعيين ملف تعريف لجهاز المستخدم الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="807f9-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="807f9-113">إذا لم يتم تعيين اي ملف تعريف ، فلن يتمكن Intune من التحقق من حاله توافق الجهاز.</span><span class="sxs-lookup"><span data-stu-id="807f9-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="807f9-114">تحرير تعيين الوصول الشرطي الخاص بالمستخدم.</span><span class="sxs-lookup"><span data-stu-id="807f9-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="807f9-115">في مدخل Azure ، انتقل إلى \*\* \> \> نهج الوصول المشروط ل Intune\*\*</span><span class="sxs-lookup"><span data-stu-id="807f9-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="807f9-116">تحديد نهج من القائمة</span><span class="sxs-lookup"><span data-stu-id="807f9-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="807f9-117">انقر فوق **المستخدمون والمجموعات**</span><span class="sxs-lookup"><span data-stu-id="807f9-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="807f9-118">لاستهداف نهج معين في شخص ما ، أضفه إلى قائمه **التضمين** .</span><span class="sxs-lookup"><span data-stu-id="807f9-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="807f9-119">للتاكد من حذف شخص من النهج ، أضفه إلى قائمه **الاستبعاد** .</span><span class="sxs-lookup"><span data-stu-id="807f9-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="807f9-120">أقرا [المزيد: كيفيه مراقبه أجهزه الوصول الشرطية](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="807f9-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

