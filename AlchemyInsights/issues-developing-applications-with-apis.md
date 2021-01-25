---
title: مشاكل تطوير التطبيقات باستخدام واجات برمجه التطبيقات
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
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974205"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="21451-102">مشاكل تطوير التطبيقات باستخدام واجات برمجه التطبيقات</span><span class="sxs-lookup"><span data-stu-id="21451-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="21451-103">للبدء باستخدام واجهه برمجه التطبيق الخاصة ب Azure Active Directory ، راجع [دليل AZURE Ad GRAPH api تشغيل](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ، أو اعرض [الوثائق التبادلية التفاعلية ل azure ad graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="21451-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="21451-104">**نهاية دعم مكتبه المصادقة ل Azure Active directory (ADAL) و Azure AD Graph API (رسم البياني AAD)**</span><span class="sxs-lookup"><span data-stu-id="21451-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="21451-105">**يبدا يوم 30 يونيو ، 2020**، لن نضيف اي ميزات جديده إلى الرسم البياني ADAL و Azure AD.</span><span class="sxs-lookup"><span data-stu-id="21451-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="21451-106">سنستمر في توفير الدعم التقني وتحديثات الأمان ولكنه لن يوفر تحديثات الميزات بعد الآن.</span><span class="sxs-lookup"><span data-stu-id="21451-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="21451-107">**بدءا من 30 يونيو 2022**، سنقوم بإنهاء الدعم ل ADAL والرسم البياني ل Azure AD ولن يعود بحاجه إلى توفير الدعم التقني أو تحديثات الأمان.</span><span class="sxs-lookup"><span data-stu-id="21451-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="21451-108">ستستمر التطبيقات التي تستخدم ADAL في إصدارات نظام التشغيل الموجودة في العمل بعد هذه المرة ولكن لن تحصل علي اي دعم تقني أو تحديثات أمان.</span><span class="sxs-lookup"><span data-stu-id="21451-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="21451-109">قد لا تتلقي التطبيقات التي تستخدم الرسم البياني Azure AD بعد هذه الفترة الاستجابات من نقطه نهاية الرسم البيانية في Azure AD.</span><span class="sxs-lookup"><span data-stu-id="21451-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="21451-110">**الترحيل ADAL**</span><span class="sxs-lookup"><span data-stu-id="21451-110">**ADAL Migration**</span></span>

<span data-ttu-id="21451-111">نوصي بالتحديث إلى [مكتبه مصادقه Microsoft (مسال)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)، التي تحتوي علي أحدث الميزات وتحديثات الأمان.</span><span class="sxs-lookup"><span data-stu-id="21451-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="21451-112">إذا كنت تستخدم تطبيقات Microsoft ، فتعرف ان Microsoft يجري عمليه ترحيل تطبيقاته إلى مسال بواسطة الموعد النهائي لنهاية الدعم ، مما يضمن توفرها من الأمان وتحسينات الميزات المسالة.</span><span class="sxs-lookup"><span data-stu-id="21451-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="21451-113">[أقرا الاسئله المتداولة حول ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="21451-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="21451-114">[تعرف علي كيفيه ترحيل التطبيقات علي أساس كل نظام أساسي](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="21451-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="21451-115">إذا كنت بحاجه إلى مساعده في التعرف علي التعليمات البرمجية الخاصة بالتطبيقات التي تستخدمها ADAL ، فمن المستحسن مراجعه جميع برامج المصدر الخاصة بكل تطبيق ، والوصول إلى اي إيسفس أو موفري تطبيقات.</span><span class="sxs-lookup"><span data-stu-id="21451-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="21451-116">يمكن ان يوفر لك دعم Microsoft أيضا قائمه بكل تطبيقات ADAL التابعة ل Microsoft في نطاق المستاجر الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="21451-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="21451-117">**ترحيل الرسم البياني AAD**</span><span class="sxs-lookup"><span data-stu-id="21451-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="21451-118">بالنسبة إلى التطبيقات التي تستخدم الرسم البياني Azure AD ، اتبع الإرشادات الخاصة بنا لترحيل [تطبيقات الرسومات البيانية في AZURE ad إلى Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="21451-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="21451-119">[توفر قائمه الاختيار الخاصة بالترحيل نقطه بدء](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="21451-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="21451-120">يعرض مدخل تسجيلك في Azure app التطبيقات التي تستخدم الرسم البياني AAD.</span><span class="sxs-lookup"><span data-stu-id="21451-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="21451-121">نوصي بمراجعه كل التعليمات البرمجية المصدر لتطبيقاتك ، وإذا كان ذلك ممكنا ، فيمكنك الوصول إلى اي إيسفس أو موفري التطبيق.</span><span class="sxs-lookup"><span data-stu-id="21451-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="21451-122">يمكن ان يوفر لك دعم Microsoft أيضا قائمه بكل استخدامات الرسم البياني ل AAD في المستاجر.</span><span class="sxs-lookup"><span data-stu-id="21451-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="21451-123">بالنسبة إلى التطبيق للوصول إلى البيانات في Microsoft Graph ، يجب ان يمنح المستخدم أو المسؤول الأذونات الصحيحة عبر عمليه الموافقة.</span><span class="sxs-lookup"><span data-stu-id="21451-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="21451-124">يسرد [مرجع أذونات Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) الأذونات المقترنة بكل مجموعه رئيسيه من واجات برمجه تطبيقات microsoft graph.</span><span class="sxs-lookup"><span data-stu-id="21451-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="21451-125">يوفر أيضا إرشادات حول كيفيه استخدام الأذونات.</span><span class="sxs-lookup"><span data-stu-id="21451-125">It also provides guidance about how to use the permissions.</span></span>
