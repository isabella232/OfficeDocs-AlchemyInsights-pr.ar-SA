---
title: المشكلات المتعلقة بالارتباطات وعناوين URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707869"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="2be1f-102">المشكلات المتعلقة بالارتباطات وعناوين URL</span><span class="sxs-lookup"><span data-stu-id="2be1f-102">Issues with links and URLs</span></span>

<span data-ttu-id="2be1f-103">عنوان URL لإعادة التوجيه، أو عناوين URL للردود (وكلا التعبيرين مرادف للآخر)، هي عناوين URL التي يستخدمها النظام الأساسي للهويات في Microsoft في إرجاع الرموز المميزة التي يطلبها التطبيق.</span><span class="sxs-lookup"><span data-stu-id="2be1f-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="2be1f-104">للاطلاع على معلومات حول عناوين URL هذه، راجع المقالات التالية:</span><span class="sxs-lookup"><span data-stu-id="2be1f-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="2be1f-105">[عمليات تدفق المصادقة وسيناريوهات التطبيق](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - معلومات حول عناوين URL لإعادة التوجيه في صفحة **تسجيل التطبيق** لكل سيناريو.</span><span class="sxs-lookup"><span data-stu-id="2be1f-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="2be1f-106">القيود والحدود لعنوان URL لإعادة التوجيه أو عناوين URL للردود</span><span class="sxs-lookup"><span data-stu-id="2be1f-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="2be1f-107">**لا أعرف كيفية تسجيل عنوان URL الصحيح لإعادة التوجيه، أو عناوين URL للردود، من أجل التطبيق**</span><span class="sxs-lookup"><span data-stu-id="2be1f-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="2be1f-108">عندما تسجّل الدخول باستخدام التطبيق الذي تعمل على تطويره، إذا تم عرض مربع حوار تسجيل الدخول الرسالة التالية **AADSTS50011: عنوان URL للرد المحدد في الطلب لا يطابق عناوين URL للردود التي تم تكوينها للتطبيق <your app ID>**، فسوف يلزمك أن تضيف إلى تسجيل التطبيق عنوان URL لإعادة التوجيه والذي استخدمته تعليماتك البرمجية في طلب الرمز المميز المُقدَّم إلى النظام الأساسي للهويات في Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2be1f-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="2be1f-109">لإضافة عنوان URL للردود، انتقل إلى علامة تبويب **مصادقة** في صفحة **تسجيل التطبيق** لديك في مدخل Azure، وأضِف إدخالاَ في المقطع **عناوين URL لإعادة التوجيه**.</span><span class="sxs-lookup"><span data-stu-id="2be1f-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="2be1f-110">تعتمد القيمة التي يلزم إدخالها على نوع التطبيق الذي تنشئه، كما هو موضح أدناه:</span><span class="sxs-lookup"><span data-stu-id="2be1f-110">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="2be1f-111">بالنسبة للتطبيقات وتطبيقات الويب ذات الصفحة الواحدة، يكون عنوان URL للرد هو عنوان URL في تطبيقك.</span><span class="sxs-lookup"><span data-stu-id="2be1f-111">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="2be1f-112">راجع [تسجيل تطبيق من صفحة واحدة](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) أو [تسجيل تطبيق ويب باستخدام مدخل Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="2be1f-112">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="2be1f-113">بالنسبة لتطبيقات سطح المكتب، تعتمد القيمة التي يلزم اختيارها على:</span><span class="sxs-lookup"><span data-stu-id="2be1f-113">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="2be1f-114">النظام الأساسي (يختلف نظام MacOS عن Windows أو Linux)</span><span class="sxs-lookup"><span data-stu-id="2be1f-114">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="2be1f-115">طريقة الحصول على الرمز المميز (بشكل تفاعلي، أو باستخدام تدفق رموز الجهاز، أو باستخدام مصادقة Windows المتكاملة [IWA]، أو باستخدام اسم المستخدم/كلمة المرور).</span><span class="sxs-lookup"><span data-stu-id="2be1f-115">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="2be1f-116">للاطلاع على التفاصيل، راجع [تطبيقات سطح المكتب - تسجيل التطبيق - عناوين URL لإعادة التوجيه](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="2be1f-116">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="2be1f-117">بالنسبة لتطبيقات الأجهزة المحمولة، تعتمد عناوين URL لإعادة التوجيه على:</span><span class="sxs-lookup"><span data-stu-id="2be1f-117">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="2be1f-118">النظام الأساسي (iOS/Android/UWP)</span><span class="sxs-lookup"><span data-stu-id="2be1f-118">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="2be1f-119">المعلومات المُستخدمة في إنشاء التطبيق، مثل معرّف المجموعة في نظام التشغيل iOS واسم الحزمة وتجزئة التوقيع، تساعدك في تسجيل تطبيق مدخل Azure على نظام التشغيل Android.</span><span class="sxs-lookup"><span data-stu-id="2be1f-119">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="2be1f-120">للاطلاع على التفاصيل، راجع [تكوين النظام الأساسي وعناوين URL لإعادة التوجيه](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="2be1f-120">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="2be1f-121">واجهات برمجة تطبيقات الويب وبعض الطرق التلقائية للحصول على الرموز المميزة (مصادقة Windows المتكاملة واسم المستخدم/كلمة المرور) إلا تتطلب عنوان URL لإعادة التوجيه.</span><span class="sxs-lookup"><span data-stu-id="2be1f-121">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="2be1f-122">**لقد نشرت تطبيق الويب الخاص بي، وعند اختبار التطبيق المنشور أجد رسالة تفيد بعدم تطابق عنوان URL للردود**</span><span class="sxs-lookup"><span data-stu-id="2be1f-122">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="2be1f-123">يمكنك إضافة عناوين URL لإعادة التوجيه لكل المواقع التي تنشر فيها تطبيق الويب الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="2be1f-123">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="2be1f-124">للحصول على مزيد من المعلومات، راجع [تسجيل تطبيق ويب باستخدام مدخل Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span><span class="sxs-lookup"><span data-stu-id="2be1f-124">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="2be1f-125">يمكنك إضافة عناوين URL لإعادة التوجيه لأحد المواقع مباشرةً بعد نشر التطبيق في ذلك الموقع.</span><span class="sxs-lookup"><span data-stu-id="2be1f-125">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="2be1f-126">**لا يمكنني تسجيل عدد كافٍ من عناوين URL للردود**</span><span class="sxs-lookup"><span data-stu-id="2be1f-126">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="2be1f-127">أنت مورد برامج مستقل ولديك واحد أو أكثر من عناوين URL لإعادة التوجيه لكل عميل لديك.</span><span class="sxs-lookup"><span data-stu-id="2be1f-127">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="2be1f-128">أنت تريد الترحيل من ADAL/Azure AD v1.0 إلى MSAL/النظام الأساسي للهويات في Microsoft، ووصلت إلى [أقصى عدد من عناوين URL لإعادة التوجيه](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="2be1f-128">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="2be1f-129">لحل هذه المشكلة، [أضِف عناوين URL لإعادة التوجيه إلى أساسيات الخدمة](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) التي تتوافق مع كل عميل من عملائك.</span><span class="sxs-lookup"><span data-stu-id="2be1f-129">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
