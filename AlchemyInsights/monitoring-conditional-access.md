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
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366415"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="3482d-102">مراقبه الوصول الشرطي ل Exchange</span><span class="sxs-lookup"><span data-stu-id="3482d-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="3482d-103">سيتلقى المستخدمون الذين يستهدفون access الشرطي بريدا الكترونيا للاعلام إذا لم يستوفوا متطلبات الوصول الخاصة بمؤسسك.</span><span class="sxs-lookup"><span data-stu-id="3482d-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="3482d-104">لحل هذه المشكلة ، نوصي باجراء واحد أو أكثر من الحلول التالية:</span><span class="sxs-lookup"><span data-stu-id="3482d-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="3482d-105">إذا كان الجهاز بريسوميد بالتسجيل ، فيمكنك اشعار المستخدم بالانتقال إلى تطبيق مدخل الشركة والتحقق من انه يظهر في مدخل الشركة.</span><span class="sxs-lookup"><span data-stu-id="3482d-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="3482d-106">إذا لم يكن كذلك ، فيجب علي المستخدم تسجيل الجهاز.</span><span class="sxs-lookup"><span data-stu-id="3482d-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="3482d-107">في مدخل Azure ، انتقل إلى التوافق مع جهاز Intune >.</span><span class="sxs-lookup"><span data-stu-id="3482d-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="3482d-108">ضمن جهاز العرض ، انقر فوق توافق الجهاز.</span><span class="sxs-lookup"><span data-stu-id="3482d-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="3482d-109">اعرض تقرير توافق الاجهزه للتحقق من انه تم وضع علامة علي جهاز المستخدم علي انه متوافق.</span><span class="sxs-lookup"><span data-stu-id="3482d-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="3482d-110">في مدخل Azure ، انتقل إلى التوافق مع جهاز Intune >.</span><span class="sxs-lookup"><span data-stu-id="3482d-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="3482d-111">ضمن أداره ، انقر فوق النهج.</span><span class="sxs-lookup"><span data-stu-id="3482d-111">Under Manage, click Policies.</span></span> <span data-ttu-id="3482d-112">في قائمه نهج التوافق ، تحقق من انه تم تعيين ملف تعريف لجهاز المستخدم الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="3482d-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="3482d-113">إذا لم يتم تعيين اي ملف تعريف ، فلن يتمكن Intune من التحقق من حاله توافق الجهاز.</span><span class="sxs-lookup"><span data-stu-id="3482d-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="3482d-114">تحرير تعيين الوصول الشرطي الخاص بالمستخدم.</span><span class="sxs-lookup"><span data-stu-id="3482d-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="3482d-115">في مدخل Azure ، انتقل إلى **Intune**  >  **نهج الوصول المشروط**ل Intune  >  **Policies**.</span><span class="sxs-lookup"><span data-stu-id="3482d-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="3482d-116">حدد نهجا من القائمة.</span><span class="sxs-lookup"><span data-stu-id="3482d-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="3482d-117">انقر فوق المستخدمون والمجموعات.</span><span class="sxs-lookup"><span data-stu-id="3482d-117">Click Users and groups.</span></span>
4. <span data-ttu-id="3482d-118">لاستهداف نهج معين في شخص ما ، أضفه إلى قائمه التضمين.</span><span class="sxs-lookup"><span data-stu-id="3482d-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="3482d-119">للتاكد من حذف شخص من النهج ، أضفه إلى قائمه الاستبعاد.</span><span class="sxs-lookup"><span data-stu-id="3482d-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="3482d-120">الارتباطات المفيدة:</span><span class="sxs-lookup"><span data-stu-id="3482d-120">Helpful links:</span></span>

[<span data-ttu-id="3482d-121">نظره عامه علي توافق الاجهزه</span><span class="sxs-lookup"><span data-stu-id="3482d-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="3482d-122">استكشاف أخطاء المراجع المصدقة</span><span class="sxs-lookup"><span data-stu-id="3482d-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="3482d-123">نهج استكشاف الأخطاء وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="3482d-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="3482d-124">مراقبه توافق جهاز Intune</span><span class="sxs-lookup"><span data-stu-id="3482d-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="3482d-125">ملاحظه: هذه الخطوات مفيده فقط في استكشاف الأخطاء وإصلاحها في الوصول الشرطي لميزه Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3482d-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="3482d-126">من الممكن أيضا اجراء فحص للجهاز حظر الوصول إلى البريد الكتروني باستخدام نهج Exchange.</span><span class="sxs-lookup"><span data-stu-id="3482d-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="3482d-127">يمكن العثور علي مزيد من المعلومات حول أداره أجهزه Exchange [هنا](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="3482d-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
