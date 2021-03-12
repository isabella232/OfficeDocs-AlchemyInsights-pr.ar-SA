---
title: مراقبة الوصول المشروط
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708661"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="2d3fe-102">مراقبة الوصول الشرطي ل Exchange</span><span class="sxs-lookup"><span data-stu-id="2d3fe-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="2d3fe-103">سيتلقى المستخدمون المستهدفون الذين لديهم وصول مشروط رسالة بريد إلكتروني إعلام إذا لم يلبيوا متطلبات الوصول إلى مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="2d3fe-104">لحل هذه المشكلة، نوصي باستخدام حل واحد أو أكثر من الحلول التالية:</span><span class="sxs-lookup"><span data-stu-id="2d3fe-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="2d3fe-105">إذا كان من المفترض أن يتم تسجيل الجهاز، فنصح المستخدمين بأن يرحلوا إلى تطبيق Company Portal وتحقق من ظهوره في Company Portal.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="2d3fe-106">وإذا لم يحدث ذلك، يجب على المستخدم تسجيل الجهاز.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="2d3fe-107">في مدخل Azure، انتقل إلى Intune > توافق الجهاز.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="2d3fe-108">ضمن "جهاز العرض"، انقر فوق توافق الجهاز.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="2d3fe-109">اشاهد تقرير توافق الجهاز للتحقق من وضع علامة على جهاز المستخدم كمتوافق.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="2d3fe-110">في مدخل Azure، انتقل إلى Intune > توافق الجهاز.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="2d3fe-111">ضمن "إدارة"، انقر فوق "سياسات".</span><span class="sxs-lookup"><span data-stu-id="2d3fe-111">Under Manage, click Policies.</span></span> <span data-ttu-id="2d3fe-112">في قائمة سياسات التوافق، تحقق من تعيين ملف تعريف إلى جهاز المستخدم.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="2d3fe-113">إذا لم يتم تعيين ملف تعريف، لن يتمكن Intune من تأكيد حالة توافق الجهاز.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="2d3fe-114">تحرير تعيين الوصول المشروط للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="2d3fe-115">في مدخل Azure، انتقل إلى "سياسات الوصول المشروط إلى **Intune".**  >    >  </span><span class="sxs-lookup"><span data-stu-id="2d3fe-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="2d3fe-116">حدد نهج من القائمة.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="2d3fe-117">انقر فوق المستخدمين والمجموعات.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-117">Click Users and groups.</span></span>
4. <span data-ttu-id="2d3fe-118">لاستهداف نهج معين لأحد الأشخاص، أضفه إلى القائمة "تضمين".</span><span class="sxs-lookup"><span data-stu-id="2d3fe-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="2d3fe-119">للتأكد من حذف شخص من النهج، أضفه إلى القائمة "استبعاد".</span><span class="sxs-lookup"><span data-stu-id="2d3fe-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="2d3fe-120">ارتباطات مفيدة:</span><span class="sxs-lookup"><span data-stu-id="2d3fe-120">Helpful links:</span></span>

[<span data-ttu-id="2d3fe-121">نظرة عامة حول توافق الجهاز</span><span class="sxs-lookup"><span data-stu-id="2d3fe-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="2d3fe-122">استكشاف الأخطاء الم CA وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="2d3fe-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="2d3fe-123">نهج استكشاف الأخطاء وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="2d3fe-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="2d3fe-124">مراقبة توافق أجهزة Intune</span><span class="sxs-lookup"><span data-stu-id="2d3fe-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="2d3fe-125">ملاحظة: هذه الخطوات مفيدة فقط في استكشاف الأخطاء في ميزة الوصول المشروط ل Azure Active Directory وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="2d3fe-126">من الممكن أيضا فحص جهاز يمنع الوصول إلى البريد الإلكتروني الخاص به باستخدام نهج Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d3fe-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="2d3fe-127">يمكن العثور على مزيد من المعلومات حول إدارة أجهزة Exchange [هنا]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="2d3fe-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
