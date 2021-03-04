---
title: استكشاف الأخطاء في SSPR وإصلاحها
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429284"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="34861-102">استكشاف الأخطاء في SSPR وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="34861-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="34861-103">**أواجه مشكلة في تكوين إعادة تعيين كلمة المرور**</span><span class="sxs-lookup"><span data-stu-id="34861-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="34861-104">إذا كنت مسؤولا وتبحث عن كيفية تمكين إعادة تعيين كلمة المرور ذاتي الخدمة، فشاهد البرنامج التعليمي لتمكين [SSPR،](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)لتكوين إعادة تعيين كلمة المرور لم مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="34861-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="34861-105">قد تحتاج أيضا إلى مراجعة [متطلبات الترخيص.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="34861-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="34861-106">يجب أن يكون لديك ترخيص واحد على الأقل تم تعيينه في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="34861-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="34861-107">**مستخدمو السحابة فقط** - أي SKU مدفوعة من Office 365 (O365) أو Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="34861-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="34861-108">المستخدمون في السحابة **و/أو** المحليون - Azure AD Premium P1 أو P2 أو Enterprise Mobility + Security (EMS) أو Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="34861-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="34861-109">لمزيد من الأسئلة حول إعادة تعيين كلمة مرور الخدمة الذاتية، راجع [الأسئلة الشائعة.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="34861-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="34861-110">**أتلقى رسالة خطأ**</span><span class="sxs-lookup"><span data-stu-id="34861-110">**I'm getting an error message**</span></span>

<span data-ttu-id="34861-111">راجع هذه المقالة للعثور على الأخطاء الشائعة وحلولها: استكشاف أخطاء إعادة تعيين كلمة مرور الخدمة الذاتية [وإصلاحها](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="34861-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="34861-112">**أواجه مشكلة في نهج إعادة تعيين كلمة المرور**</span><span class="sxs-lookup"><span data-stu-id="34861-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="34861-113">إذا لم يكن نهج إعادة تعيين كلمة المرور قيد التشغيل كما هو متوقع، أو إذا كانت لديك أسئلة حول نهج إعادة تعيين كلمة المرور، فراجع هذه المقالة: نهج كلمات المرور والقيود في [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="34861-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="34861-114">لا تنطبق سياسات إعادة تعيين كلمة المرور على المسؤولين.</span><span class="sxs-lookup"><span data-stu-id="34861-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="34861-115">تفرض Microsoft نهج إعادة تعيين كلمة مرور افتراضية وقوية ذات بوابة لأي دور مسؤول Azure.</span><span class="sxs-lookup"><span data-stu-id="34861-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="34861-116">تأكد من أنك تقوم باختباره مع مستخدم ليس مسؤولا.</span><span class="sxs-lookup"><span data-stu-id="34861-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="34861-117">لمزيد من المعلومات حول نهج إعادة تعيين المسؤول، راجع هذه المقالة: إعادة تعيين المسؤول [لاختلافات النهج.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="34861-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="34861-118">**لا أريد أن يسجل المستخدمون معلومات أمان إضافية لإعادة تعيين كلمة المرور**</span><span class="sxs-lookup"><span data-stu-id="34861-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="34861-119">يمكنك تعبئة البيانات مسبقا (سمات البريد الإلكتروني والهاتف) للمستخدمين باستخدام API أو PowerShell أو Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="34861-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="34861-120">لمعرفة كيفية القراءة:</span><span class="sxs-lookup"><span data-stu-id="34861-120">To learn how read:</span></span>

- [<span data-ttu-id="34861-121">نشر إعادة تعيين كلمة المرور دون مطالبة المستخدمين بالتسجيل</span><span class="sxs-lookup"><span data-stu-id="34861-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="34861-122">البيانات التي تستخدمها إعادة تعيين كلمة المرور</span><span class="sxs-lookup"><span data-stu-id="34861-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="34861-123">**أريد أن يسجل المستخدمون معلومات الأمان الإضافية لإعادة تعيين كلمة المرور**</span><span class="sxs-lookup"><span data-stu-id="34861-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="34861-124">يجب على المستخدمين تسجيل معلومات الأمان لإعادة تعيين كلمة مرور الخدمة الذاتية عن طريق توجيههم إلى [aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)</span><span class="sxs-lookup"><span data-stu-id="34861-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="34861-125">بعد تعبئة البيانات للمستخدم (بواسطة المستخدم أو المسؤول)، قم توجيه [](https://passwordreset.microsoftonline.com/) المستخدم إلى aka.ms/sspr بحيث يمكن تمكين المستخدمين من إعادة تعيين كلمات المرور الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="34861-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="34861-126">إذا كان المستخدمون لا يزالوا  يعانون من مشاكل، فهم على المرجح أن يكونوا مستخدمين موحوحين أو مزامنتهم بكلمات **مرور.**</span><span class="sxs-lookup"><span data-stu-id="34861-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="34861-127">وهذا يعني أنه من المرجح وجود مشكلة في خدمة "كتابة كلمة المرور".</span><span class="sxs-lookup"><span data-stu-id="34861-127">This means there is likely a problem with the Password Writeback service.</span></span>