---
title: تطبيق المصادقة
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404187"
---
# <a name="authentication-app"></a><span data-ttu-id="69e4c-102">تطبيق المصادقة</span><span class="sxs-lookup"><span data-stu-id="69e4c-102">Authentication app</span></span>

<span data-ttu-id="69e4c-103">إذا كنت المسؤول العام، يمكنك بسرعة معرفة ما حدث أو تشخيص المشاكل المتعلقة تسجيل الدخول من قبل المستخدم باستخدام تشخيص تسجيل [الدخول](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="69e4c-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="69e4c-104">ابدأ التشخيص بالنقر فوق الزر["تشغيل التشخيص".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="69e4c-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="69e4c-105">ابحث عن الحدث الذي تريد تحليله بإدخال التفاصيل التي لديك حول المستخدم أو التطبيق أو وقت تسجيل الدخول أو طلب المعرف أو المعرف الارتباطي.</span><span class="sxs-lookup"><span data-stu-id="69e4c-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="69e4c-106">راجع نتائج التشخيص التي تظهر تفاصيل ما حدث والإجراءات التي يمكنك اتخاذها من أجل إجراء تغييرات، إذا كانت هناك حاجة إلى أي تغييرات.</span><span class="sxs-lookup"><span data-stu-id="69e4c-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="69e4c-107">**تحقق من السيناريو الذي ينطبق:**</span><span class="sxs-lookup"><span data-stu-id="69e4c-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="69e4c-108">إذا لم يحصل المستخدم على إعلام في تطبيق Microsoft Authenticator، فتحقق من عدم إظهاره ضمن المستخدمين المحظورين ل MFA كما هو موضح في حظر المستخدمين و إلغاء [حظرهم.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="69e4c-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="69e4c-109">إذا لم يتم حظر المستخدم ل MFA ولكنه لم يتلق إعلاما، يمكنه فتح تطبيق Microsoft Authenticator، الذي سيسحب طلبات الموافقة المعلقة.</span><span class="sxs-lookup"><span data-stu-id="69e4c-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="69e4c-110">كطريقة بديلة تسجيل الدخول، يمكن للمستخدم أيضا النقر فوق تسجيل الدخول بطريقة أخرى واختيار استخدام رمز التحقق من صحة من تطبيق الأجهزة المحمولة.</span><span class="sxs-lookup"><span data-stu-id="69e4c-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="69e4c-111">تطبيق Microsoft Authenticator هو الأسلوب الوحيد المتوفر للعديد من المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="69e4c-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="69e4c-112">[تعرف على المزيد حول إعدادات الأمان الافتراضية](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)، تحقق من الأسئلة الشائعة حول الأسئلة الشائعة حول تطبيق [المصادقة](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) وكيفية حلها.</span><span class="sxs-lookup"><span data-stu-id="69e4c-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="69e4c-113">**مقاطع الفيديو المستحسنة**</span><span class="sxs-lookup"><span data-stu-id="69e4c-113">**Recommended Videos**</span></span>

<span data-ttu-id="69e4c-114">[كيفية إعداد تطبيق Authenticator على هاتف جديد (2 دقيقة)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="69e4c-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
