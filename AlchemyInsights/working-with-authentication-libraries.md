---
title: استخدام مكتبات المصادقة
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034754"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="959b8-102">استخدام مكتبات المصادقة</span><span class="sxs-lookup"><span data-stu-id="959b8-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="959b8-103">لحل مشكلة مكتبة مصادقة Microsoft (MSAL)، يجب تنفيذ الخطوات الموصى بها التالية:</span><span class="sxs-lookup"><span data-stu-id="959b8-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="959b8-104">**استخدام MSAL**: [مكتبات](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) مصادقة النظام الأساسي لهوية Microsoft - تعرض هذه المقالة دعم مكتبة مصادقة Microsoft لأنواع تطبيقات متعددة.</span><span class="sxs-lookup"><span data-stu-id="959b8-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="959b8-105">ويتضمن ارتباطات إلى التعليمات البرمجية المصدر للمكتبة؛ مكان الحصول على حزمة لمشروع تطبيقك؛ وما إذا كانت المكتبة تدعم تسجيل دخول المستخدم (المصادقة) أو الوصول إلى واجهات برمجة تطبيقات الويب المحمية (التخويل) أو كليهما.</span><span class="sxs-lookup"><span data-stu-id="959b8-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="959b8-106">**استكشاف الأخطاء وإصلاحها المصادقة**: تدعم MSAL العديد من تدفقات المصادقة لاستخدامها في سيناريوهات تطبيق مختلفة.</span><span class="sxs-lookup"><span data-stu-id="959b8-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="959b8-107">استنادا إلى كيفية إنشاء تطبيق العميل، يمكن ل MSAL استخدام واحد أو أكثر من تدفقات المصادقة المعتمدة من النظام الأساسي لهوية Microsoft.</span><span class="sxs-lookup"><span data-stu-id="959b8-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="959b8-108">يمكن لهذه التدفقات أن تنتج أنواعا متعددة من الرموز المميزة ورموز التخويل، وتتطلب رموزا مميزا مختلفة لجعلها تعمل.</span><span class="sxs-lookup"><span data-stu-id="959b8-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="959b8-109">**رموز Access** المميزة : الرموز المميزة للوصول إلى النظام الأساسي لهوية [Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - تعرف على كيفية التحقق من صحة API واستخدام المطالبات داخل رمز الوصول المميز.</span><span class="sxs-lookup"><span data-stu-id="959b8-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="959b8-110">تنطبق كل الوثائق في هذه المقالة، باستثناء الوثائق التي تم ذكرها، فقط على الرموز المميزة التي تم إصدارها ل واجهات برمجة التطبيقات التي قمت بتسجيلها.</span><span class="sxs-lookup"><span data-stu-id="959b8-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="959b8-111">ولا ينطبق على الرموز المميزة التي تم إصدارها ل واجهات برمجة التطبيقات المملوكة ل Microsoft، ولا يمكن استخدام هذه الرموز المميزة للتحقق من كيفية إصدار النظام الأساسي لهوية Microsoft الرموز المميزة ل API التي تقوم بإنشاءها.</span><span class="sxs-lookup"><span data-stu-id="959b8-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="959b8-112">**انتهاء الدعم لمكتبة مصادقة Azure Active Directory (ADAL)**</span><span class="sxs-lookup"><span data-stu-id="959b8-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="959b8-113">**اعتبارا من 30 يونيو 2020،** لن نضيف أي ميزات جديدة إلى ADAL و Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="959b8-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="959b8-114">سنستمر في تقديم الدعم الفني وتحديثات الأمان ولكننا لن نقدم تحديثات للميزات بعد الآن.</span><span class="sxs-lookup"><span data-stu-id="959b8-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="959b8-115">**اعتبارا من 30 يونيو 2022،** سننهي دعم ADAL و Azure AD Graph ولن نوفر تحديثات الأمان أو الدعم التقني.</span><span class="sxs-lookup"><span data-stu-id="959b8-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="959b8-116">ستستمر التطبيقات التي تستخدم ADAL على إصدارات نظام التشغيل الموجودة في العمل بعد هذا الوقت ولكنها لن تحصل على أي تحديثات أمنية أو *دعم تقني.*</span><span class="sxs-lookup"><span data-stu-id="959b8-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="959b8-117">قد لا تتلقى التطبيقات التي تستخدم Azure AD Graph بعد هذا الوقت استجابات من نقطة نهاية Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="959b8-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="959b8-118">**ترحيل ADAL**</span><span class="sxs-lookup"><span data-stu-id="959b8-118">**ADAL Migration**</span></span>

- <span data-ttu-id="959b8-119">نوصي بالتحديث إلى MSAL، الذي يضم أحدث الميزات وتحديثات الأمان.</span><span class="sxs-lookup"><span data-stu-id="959b8-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="959b8-120">إذا كنت تستخدم تطبيقات Microsoft، فتعرف على أن Microsoft تقوم بتهجر تطبيقاتها إلى MSAL بحلول الموعد النهائي لنهاية الدعم، مع التأكد من أنها ستستفيد من تحسينات الميزات والأمان المستمرة ل MSAL.</span><span class="sxs-lookup"><span data-stu-id="959b8-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="959b8-121">[اقرأ الأسئلة الشائعة حول ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="959b8-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="959b8-122">[تعرف على كيفية ترحيل التطبيقات على أساس كل نظام أساسي.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)</span><span class="sxs-lookup"><span data-stu-id="959b8-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="959b8-123">إذا كانت لديك أسئلة إضافية بعد قراءة دليل النظام الأساسي للتطبيق، يمكنك النشر على [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) باستخدام العلامة [azure-ad-adal-deprecation] أو فتح مشكلة في مستودع GitHub الخاص بالمكتبة.</span><span class="sxs-lookup"><span data-stu-id="959b8-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="959b8-124">راجع [القسم اللغات وأطر العمل من](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) مقالة نظرة **عامة حول MSAL** للحصول على ارتباطات إلى إعادة نشر كل مكتبة.</span><span class="sxs-lookup"><span data-stu-id="959b8-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="959b8-125">إذا كنت بحاجة إلى مساعدة في فهم التطبيقات التي تستخدم **ADAL،** فإننا ننصحك بمراجعة كل التعليمات البرمجية المصدر لتطبيقاتك.</span><span class="sxs-lookup"><span data-stu-id="959b8-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="959b8-126">إذا كان ذلك قابلا للتطبيق، يمكنك التواصل مع أي موردي برامج مستقلة (ISVs) أو موفري التطبيقات.</span><span class="sxs-lookup"><span data-stu-id="959b8-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="959b8-127">يمكن أن يوفر لك دعم Microsoft أيضًا قائمة بجميع تطبيقات ADAL غير التابعة لـ Microsoft في المستأجر الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="959b8-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







