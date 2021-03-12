---
title: مشاكل Microsoft Graph API
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/29/2021
ms.locfileid: "50713296"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="b7d8a-102">مشاكل Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="b7d8a-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="b7d8a-103">قد ينطبق هذا الموضوع أيضا على المطورين الذين ما زالوا يستخدمون Azure AD Graph API.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="b7d8a-104">ومع **ذلك،** يوصى بشدة باستخدام Microsoft Graph لكل سيناريوهات إدارة الدليل والهوية والوصول.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="b7d8a-105">**مشاكل المصادقة أو التفويض**</span><span class="sxs-lookup"><span data-stu-id="b7d8a-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="b7d8a-106">إذا تعذر  على تطبيقك الحصول على الرموز المميزة لاستدعاء Microsoft Graph، فاختار مشكلة في الحصول على رمز وصول **مميز (مصادقة)** فئة Microsoft Graph للحصول على تعليمات ودعم أكثر تحديدا حول هذا الموضوع.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="b7d8a-107">إذا كان التطبيق يتلقى أخطاء تخويل **401 أو 403** عند الاتصال ب Microsoft Graph، فاختار فئة Microsoft Graph API لرفض الوصول **للحصول** على تعليمات ودعم أكثر تحديدا حول هذا الموضوع.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="b7d8a-108">**أريد استخدام Microsoft Graph، ولكن لست متأكدا من مكان البدء**</span><span class="sxs-lookup"><span data-stu-id="b7d8a-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="b7d8a-109">نظرة عامة على Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b7d8a-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="b7d8a-110">نظرة عامة حول إدارة الهوية والوصول في Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b7d8a-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="b7d8a-111">بدء إنشاء تطبيقات Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b7d8a-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="b7d8a-112">**مستكشف Microsoft Graph** - اختبر واجهات برمجة تطبيقات Microsoft Graph في المستأجر أو مستأجر عرض توضيحي</span><span class="sxs-lookup"><span data-stu-id="b7d8a-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="b7d8a-113">**أريد استخدام Microsoft Graph، ولكن هل يدعم واجهات برمجة تطبيقات الدليل 1.0 التي أحتاجها؟**</span><span class="sxs-lookup"><span data-stu-id="b7d8a-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="b7d8a-114">Microsoft Graph هو API الموصى به لإدارة الدليل والهوية والوصول.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="b7d8a-115">ومع ذلك، لا تزال هناك بعض الفراغات بين ما هو ممكن في Azure AD Graph و Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="b7d8a-116">راجع المقالات التالية، التي تسلط الضوء على أحدث الاختلافات لمساعدتك في اختيارك:</span><span class="sxs-lookup"><span data-stu-id="b7d8a-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="b7d8a-117">اختلافات نوع المورد بين Azure AD Graph و Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b7d8a-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="b7d8a-118">اختلافات في الممتلكات بين Azure AD Graph و Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b7d8a-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="b7d8a-119">اختلافات الأسلوب بين Azure AD و Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b7d8a-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="b7d8a-120">**لا تعمل API التي أقوم بالاتصال بها - أين يمكنني إجراء المزيد من الاختبارات؟**</span><span class="sxs-lookup"><span data-stu-id="b7d8a-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="b7d8a-121">**مستكشف Microsoft Graph** - اختبر واجهات برمجة تطبيقات Microsoft Graph في المستأجر أو مستأجر عرض توضيحي وافحص أيضا نماذج الاستعلامات **في** Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="b7d8a-122">**تطبيقي بطيء جدا ويتلقى أيضا بعض البطء. ما هي التحسينات التي يمكنني إدخالها؟**</span><span class="sxs-lookup"><span data-stu-id="b7d8a-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="b7d8a-123">وفقا للسيناريو الخاص بك، هناك مجموعة متنوعة من الخيارات تحت تصرفك لجعل تطبيقك أكثر أداء، وفي بعض الحالات، أقل عرضة للتوقف عن الخدمة (عند إجراء عدد كبير جدا من المكالمات).</span><span class="sxs-lookup"><span data-stu-id="b7d8a-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="b7d8a-124">أفضل الممارسات في Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b7d8a-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="b7d8a-125">طلبات الدفع</span><span class="sxs-lookup"><span data-stu-id="b7d8a-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="b7d8a-126">تعقب التغييرات عبر استعلام دلتا</span><span class="sxs-lookup"><span data-stu-id="b7d8a-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="b7d8a-127">الحصول على إعلامات التغييرات من خلال هاته الويب</span><span class="sxs-lookup"><span data-stu-id="b7d8a-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="b7d8a-128">إرشادات التدويل</span><span class="sxs-lookup"><span data-stu-id="b7d8a-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="b7d8a-129">**أين يمكنني العثور على مزيد من المعلومات حول الأخطاء وا المشاكل المعروفة؟**</span><span class="sxs-lookup"><span data-stu-id="b7d8a-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="b7d8a-130">معلومات استجابة الخطأ في Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b7d8a-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="b7d8a-131">المشاكل المعروفة في Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b7d8a-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="b7d8a-132">**أين يمكنني التحقق من حالة توفر الخدمة والاتصال؟**</span><span class="sxs-lookup"><span data-stu-id="b7d8a-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="b7d8a-133">يمكن أن يؤثر توفر الخدمة واتصال الخدمات الأساسية التي يمكن الوصول إليها من خلال Microsoft Graph على التوفر والأداء العامين ل Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="b7d8a-134">للحصول على حماية خدمة Azure Active Directory، تحقق من حالة **خدمات الأمان +** الهوية المدرجة في صفحة حالة [Azure.](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="b7d8a-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="b7d8a-135">بالنسبة لخدمات Office التي تساهم في Microsoft Graph، تحقق من حالة الخدمات المدرجة في لوحة معلومات [حالة خدمة Office.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="b7d8a-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="b7d8a-136">يمكن أن تكون أخطاء تخويل Microsoft Graph ناتجة عن العديد من المشاكل المختلفة، التي ينتج عن معظمها الخطأ 401 أو 403.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="b7d8a-137">على سبيل المثال، يمكن أن يؤدي كل ما يلي إلى حدوث أخطاء التخويل:</span><span class="sxs-lookup"><span data-stu-id="b7d8a-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="b7d8a-138">[تدفقات الحصول على الرمز المميز للوصول](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios) غير صحيحة</span><span class="sxs-lookup"><span data-stu-id="b7d8a-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="b7d8a-139">[نطاقات الأذونات](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) تم تكوينها بشكل غير صحيح</span><span class="sxs-lookup"><span data-stu-id="b7d8a-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="b7d8a-140">عدم [الموافقة](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="b7d8a-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="b7d8a-141">\**_إنهاء دعم مكتبة مصادقة Azure Active Directory (ADAL) و Azure AD Graph API (AAD Graph)_* _</span><span class="sxs-lookup"><span data-stu-id="b7d8a-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="b7d8a-142">_\*بدءا من 30 يونيو 2020\*\*، لن نضيف أي ميزات جديدة إلى ADAL و Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="b7d8a-143">سنستمر في تقديم الدعم الفني وتحديثات الأمان ولكننا لن نقدم تحديثات للميزات بعد الآن.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="b7d8a-144">**اعتبارا من 30 يونيو 2022،** سننهي دعم ADAL و Azure AD Graph ولن نوفر تحديثات الأمان أو الدعم التقني.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="b7d8a-145">ستستمر التطبيقات التي تستخدم ADAL على إصدارات نظام التشغيل الموجودة في العمل بعد هذا الوقت ولكنها لن تحصل على أي تحديثات للدعم التقني *أو الأمان.*</span><span class="sxs-lookup"><span data-stu-id="b7d8a-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="b7d8a-146">قد لا تتلقى التطبيقات التي تستخدم Azure AD Graph بعد هذا الوقت استجابات من نقطة نهاية Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="b7d8a-147">**ترحيل ADAL**</span><span class="sxs-lookup"><span data-stu-id="b7d8a-147">**ADAL Migration**</span></span>

<span data-ttu-id="b7d8a-148">نوصي بالتحديث إلى [مكتبة مصادقة Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)، التي تحتوي على أحدث الميزات وتحديثات الأمان.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="b7d8a-149">إذا كنت تستخدم تطبيقات Microsoft، فتعرف على أن Microsoft تقوم بتقليل تطبيقاتها إلى MSAL بحلول الموعد النهائي لنهاية الدعم، مع التأكد من أنها ستستفيد من تحسينات الميزات والأمان المستمرة في MSAL.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="b7d8a-150">قراءة الأسئلة الشائعة حول ADAL</span><span class="sxs-lookup"><span data-stu-id="b7d8a-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="b7d8a-151">تعرّف على كيفية ترحيل التطبيقات على أساس كل نظام أساسي</span><span class="sxs-lookup"><span data-stu-id="b7d8a-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="b7d8a-152">إذا احتجت إلى مساعدة في فهم التطبيقات التي تستخدم ADAL، فإننا ننصحك بمراجعة كل التعليمات البرمجية المصدر للتطبيقات، وإذا كان ذلك قابلا للتطبيق، فصل إلى أي موفري خدمات الإنترنت أو موفري التطبيقات.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="b7d8a-153">يمكن أن يوفر لك دعم Microsoft أيضًا قائمة بجميع تطبيقات ADAL غير التابعة لـ Microsoft في المستأجر الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="b7d8a-154">**ترحيل AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="b7d8a-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="b7d8a-155">بالنسبة للتطبيقات التي تستخدم Azure AD Graph، اتبع الإرشادات الخاصة بترحيل تطبيقات [Azure AD Graph إلى Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="b7d8a-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="b7d8a-156">[توفر قائمة اختيار الترحيل نقطة بدء استخدام](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="b7d8a-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="b7d8a-157">يُُظهر مدخل تسجيل تطبيق Azure التطبيقات التي تستخدم AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="b7d8a-158">نوصيك بمراجعة جميع التعليمات البرمجية المصدر لتطبيقاتك، وإذا أمكن، يمكنك الوصول إلى أي من موردي البرامج المستقلين أو مزودي التطبيقات.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="b7d8a-159">يمكن أن يوفر لك دعم Microsoft أيضا قائمة بجميع استخدام AAD Graph في المستأجر الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="b7d8a-160">لكي يمكن لتطبيقك الوصول إلى البيانات في Microsoft Graph، يجب على المستخدم أو المسؤول منحه الأذونات الصحيحة عبر عملية موافقة.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="b7d8a-161">يسرد [مرجع أذونات Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) الأذونات المقترنة بكل مجموعة رئيسية من واجهات برمجة تطبيقات Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="b7d8a-162">كما يوفر إرشادات حول كيفية استخدام الأذونات.</span><span class="sxs-lookup"><span data-stu-id="b7d8a-162">It also provides guidance about how to use the permissions.</span></span>
