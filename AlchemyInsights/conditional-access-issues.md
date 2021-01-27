---
title: مشاكل الوصول الشرطي
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014706"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="a5f17-102">مشاكل الوصول الشرطي</span><span class="sxs-lookup"><span data-stu-id="a5f17-102">Conditional access issues</span></span>

<span data-ttu-id="a5f17-103">**حل المشاكل المتعلقة بتشخيص تسجيل الدخول**</span><span class="sxs-lookup"><span data-stu-id="a5f17-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="a5f17-104">يمكنك التعرف بسرعة علي المشاكل المتعلقة بتسجيل الدخول إلى المستخدم باستخدام " [تشخيص تسجيل الدخول](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)":</span><span class="sxs-lookup"><span data-stu-id="a5f17-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="a5f17-105">شغل تشخيص تسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="a5f17-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="a5f17-106">ابحث عن الحدث المراد تحليله عن طريق إدخال التفاصيل التي لديك بشان المستخدم أو التطبيق أو وقت تسجيل الدخول أو معرف الطلب أو معرف الارتباط.</span><span class="sxs-lookup"><span data-stu-id="a5f17-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="a5f17-107">راجع نتائج التشخيص التي تعرض تفاصيل ما حدث والإجراءات التي يمكنك اتخاذها لاجراء التغييرات (إذا كانت هناك حاجه إلى التغييرات).</span><span class="sxs-lookup"><span data-stu-id="a5f17-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="a5f17-108">**خطوات استكشاف أخطاء تسجيل الدخول وإصلاحها**</span><span class="sxs-lookup"><span data-stu-id="a5f17-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="a5f17-109">انتقل إلى صفحه تسجيل الدخول إلى Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a5f17-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="a5f17-110">تصفيه التسجيلات بواسطة المستخدم والنطاق الزمني والتطبيق والحالة وتطبيق العميل وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="a5f17-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="a5f17-111">حدد حدث تسجيل الدخول واعرض علامة تبويب Access الشرطية للاطلاع علي النهج التي تم تقييمها.</span><span class="sxs-lookup"><span data-stu-id="a5f17-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="a5f17-112">انقر فوق صف النهج لعرض تفاصيل النهج وفهم سبب التطبيق.</span><span class="sxs-lookup"><span data-stu-id="a5f17-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="a5f17-113">**أدوات لاستكشاف أخطاء نهج Access الشرطي وإصلاحها**</span><span class="sxs-lookup"><span data-stu-id="a5f17-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="a5f17-114">يتيح لك وضع التقرير فقط تقييم نهج من دون التاثير علي المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="a5f17-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="a5f17-115">أداه "ماذا إذا" تسمح لك بمحاكاة احداث تسجيل الدخول ومعرفه النهج التي تنطبق.</span><span class="sxs-lookup"><span data-stu-id="a5f17-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="a5f17-116">تعرض المعارف الدقيقة ومصنف التقارير تاثير الوقت الحقيقي لكل نهج.</span><span class="sxs-lookup"><span data-stu-id="a5f17-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="a5f17-117">**نهج حماية الأساس**</span><span class="sxs-lookup"><span data-stu-id="a5f17-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="a5f17-118">تم إهمال نهج حماية الأساس.</span><span class="sxs-lookup"><span data-stu-id="a5f17-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="a5f17-119">لم يعد يتم فرضها ستتم ازالتها قريبا من مدخل Azure.</span><span class="sxs-lookup"><span data-stu-id="a5f17-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="a5f17-120">نوصي بتمكين [إعدادات الأمان الافتراضية](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="a5f17-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="a5f17-121">للحصول علي مزيد من المعلومات حول الوصول الشرطي ، راجع:</span><span class="sxs-lookup"><span data-stu-id="a5f17-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="a5f17-122">[أفضل الممارسات للوصول الشرطي في Azure Active](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 directory [الشروط في الوصول](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 الشرطي [عناصر التحكم في Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 الشرطي [المواقع في Access الشرطي](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="a5f17-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
