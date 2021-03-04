---
title: مراقبة الوصول المشروط إلى Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/03/2021
ms.locfileid: "50426992"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="a47e1-102">مراقبة الوصول المشروط إلى Intune</span><span class="sxs-lookup"><span data-stu-id="a47e1-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="a47e1-103">سيتلقى المستخدمون المستهدفون الذين لديهم وصول شرطي بريدا إلكترونيا إعلاما إذا لم يلبيوا متطلبات الوصول إلى مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="a47e1-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="a47e1-104">لحل هذه المشكلة، نوصي باستخدام حل واحد أو أكثر من الحلول التالية:</span><span class="sxs-lookup"><span data-stu-id="a47e1-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="a47e1-105">إذا كان من المفترض أن يتم تسجيل الجهاز، فنصح المستخدمين بأن يقوموا الانتقال إلى تطبيق Company Portal وتحقق من ظهوره في Company Portal.</span><span class="sxs-lookup"><span data-stu-id="a47e1-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="a47e1-106">وإذا لم يحدث ذلك، فيجب على المستخدم تسجيل الجهاز.</span><span class="sxs-lookup"><span data-stu-id="a47e1-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="a47e1-107">في مدخل Azure، انتقل إلى **توافق جهاز Intune.**  >  </span><span class="sxs-lookup"><span data-stu-id="a47e1-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="a47e1-108">لعرض تقرير توافق الجهاز للتحقق من وضع علامة على جهاز المستخدم كمتوافق، ضمن "جهاز العرض"، انقر فوق **توافق الجهاز.**</span><span class="sxs-lookup"><span data-stu-id="a47e1-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="a47e1-109">في مدخل Azure، انتقل إلى **توافق جهاز Intune.**  >  </span><span class="sxs-lookup"><span data-stu-id="a47e1-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="a47e1-110">ضمن **"إدارة"، انقر** فوق **"سياسات".**</span><span class="sxs-lookup"><span data-stu-id="a47e1-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="a47e1-111">في قائمة سياسات التوافق، تحقق من تعيين ملف تعريف إلى جهاز المستخدم.</span><span class="sxs-lookup"><span data-stu-id="a47e1-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="a47e1-112">إذا لم يتم تعيين ملف تعريف، لن يتمكن Intune من تأكيد حالة توافق الجهاز.</span><span class="sxs-lookup"><span data-stu-id="a47e1-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="a47e1-113">تحرير تعيين الوصول المشروط للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="a47e1-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="a47e1-114">في مدخل Azure، انتقل إلى نهج الوصول المشروط في **Intune،** وحدد نهج من القائمة، وانقر فوق المستخدمين  >    >   **والمجموعات.**</span><span class="sxs-lookup"><span data-stu-id="a47e1-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="a47e1-115">لاستهداف نهج معين لأحد الأشخاص، أضفه إلى القائمة **"تضمين".**</span><span class="sxs-lookup"><span data-stu-id="a47e1-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="a47e1-116">للتأكد من حذف شخص من النهج، أضفه إلى القائمة **"استبعاد".**</span><span class="sxs-lookup"><span data-stu-id="a47e1-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="a47e1-117">**ارتباطات مفيدة:**</span><span class="sxs-lookup"><span data-stu-id="a47e1-117">**Helpful links:**</span></span>

- [<span data-ttu-id="a47e1-118">نظرة عامة حول توافق الجهاز</span><span class="sxs-lookup"><span data-stu-id="a47e1-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="a47e1-119">استكشاف الأخطاء الم CA وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="a47e1-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="a47e1-120">نهج استكشاف الأخطاء وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="a47e1-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="a47e1-121">مراقبة توافق أجهزة Intune</span><span class="sxs-lookup"><span data-stu-id="a47e1-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="a47e1-122">هذه الخطوات مفيدة فقط في استكشاف الأخطاء في ميزة الوصول المشروط ل Azure Active Directory وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="a47e1-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="a47e1-123">من الممكن أيضا فحص جهاز يمنع الوصول إلى البريد الإلكتروني الخاص به باستخدام نهج Exchange.</span><span class="sxs-lookup"><span data-stu-id="a47e1-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="a47e1-124">يمكن العثور على مزيد من المعلومات حول إدارة أجهزة Exchange [**هنا.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="a47e1-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
