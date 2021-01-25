---
title: المشاكل المتعلقة بالارتباطات وعناوين Url
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974157"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="35954-102">المشاكل المتعلقة بالارتباطات وعناوين Url</span><span class="sxs-lookup"><span data-stu-id="35954-102">Issues with links and URLs</span></span>

<span data-ttu-id="35954-103">أعاده توجيه عناوين Url للرد/الرد (يتم الآن لكل من التعبيرات) هي عناوين Url التي يستخدمها النظام الأساسي لهويه Microsoft لإرجاع الرموز المميزة المطلوبة للتطبيق.</span><span class="sxs-lookup"><span data-stu-id="35954-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="35954-104">للحصول علي معلومات حول عناوين Url هذه ، راجع المقالات التالية:</span><span class="sxs-lookup"><span data-stu-id="35954-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="35954-105">[تدفقات المصادقة وسيناريوهات التطبيقات](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) -معلومات حول معرفات uri لأعاده التوجيه في صفحه **تسجيل التطبيق** لكل سيناريو.</span><span class="sxs-lookup"><span data-stu-id="35954-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="35954-106">أعاده توجيه URI/قيود عنوان URL للرد والقيود</span><span class="sxs-lookup"><span data-stu-id="35954-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="35954-107">**لا اعرف كيفيه تسجيل عنوان URL لأعاده توجيه URI/الرد لتطبيقي**</span><span class="sxs-lookup"><span data-stu-id="35954-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="35954-108">عندما تقوم بتسجيل الدخول باستخدام التطبيق الذي تقوم بتطويره ، إذا كان مربع الحوار تسجيل الدخول يعرض **AADSTS50011: لا يتطابق عنوان url الخاص بالرد <your app ID> المحدد في الطلب علي عناوين url للرد المكونة للتطبيق**، ستحتاج إلى اضافته إلى تسجيل التطبيقات ، وهو URI لأعاده التوجيه الذي استخدمته في التعليمات</span><span class="sxs-lookup"><span data-stu-id="35954-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="35954-109">لأضافه عنوان URL للرد ، انتقل إلى علامة التبويب **المصادقة** في صفحه **تسجيل التطبيق** في Azure portal وأضف إدخالا في القسم **أعاده توجيه URIs** .</span><span class="sxs-lookup"><span data-stu-id="35954-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="35954-110">يتم كتابه معرفات Uri لأعاده التوجيه (ويب أو الهاتف المحمول/سطح المكتب).</span><span class="sxs-lookup"><span data-stu-id="35954-110">Redirect URIs are typed (Web or mobile/desktop).</span></span> <span data-ttu-id="35954-111">تعتمد القيمة التي يجب إدخالها علي نوع التطبيق الذي تقوم بإنشاءه ، كما هو موضح أدناه:</span><span class="sxs-lookup"><span data-stu-id="35954-111">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="35954-112">بالنسبة إلى تطبيقات ويب أحاديه الصفحة ، فان عنوان URL للرد هو عنوان URL في التطبيق.</span><span class="sxs-lookup"><span data-stu-id="35954-112">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="35954-113">راجع [تسجيل تطبيق الصفحة الواحد](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) أو [تسجيل تطبيق تطبيق ويب باستخدام مدخل Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="35954-113">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="35954-114">بالنسبة إلى تطبيقات سطح المكتب ، تعتمد القيمة التي يجب اختيارها علي:</span><span class="sxs-lookup"><span data-stu-id="35954-114">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="35954-115">النظام الأساسي (MacOS مختلف عن Windows أو Linux)</span><span class="sxs-lookup"><span data-stu-id="35954-115">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="35954-116">الطريقة التي تحصل فيها علي الرمز المميز (بطريقه تفاعليه ، باستخدام مصادقه Windows المتكاملة [إيفا] أو باستخدام username/password).</span><span class="sxs-lookup"><span data-stu-id="35954-116">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="35954-117">للحصول علي التفاصيل ، راجع [تطبيقات سطح المكتب-تسجيل التطبيق-أعاده توجيه URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="35954-117">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="35954-118">بالنسبة لتطبيقات الاجهزه المحمولة ، تتوقف أعاده توجيه URI علي:</span><span class="sxs-lookup"><span data-stu-id="35954-118">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="35954-119">النظام الأساسي (iOS/Android/أوب)</span><span class="sxs-lookup"><span data-stu-id="35954-119">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="35954-120">ستساعدك المعلومات المستخدمة لإنشاء التطبيق ، مثل معرف الحزمة في نظام التشغيل iOS ، سيساعدك تسجيل الدخول وتجزئه التوقيع علي Android.</span><span class="sxs-lookup"><span data-stu-id="35954-120">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="35954-121">للحصول علي التفاصيل ، راجع [تكوين النظام الأساسي وقم باعاده توجيه uri](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="35954-121">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="35954-122">واجات برمجه تطبيقات ويب وبعض الطرق الصامتة لجلب الرموز المميزة (إيفا واسم المستخدم/كلمه المرور) غير مطلوبه لأعاده توجيه URI.</span><span class="sxs-lookup"><span data-stu-id="35954-122">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="35954-123">**لقد قمت بنشر تطبيق ويب الخاص بي وعند اختبار التطبيق المنشور ، تظهر رسالة عدم تطابق عنوان url للرد**</span><span class="sxs-lookup"><span data-stu-id="35954-123">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="35954-124">أضف معرفات Uri لأعاده التوجيه لكل المواقع التي تقوم بنشر تطبيق ويب عليها.</span><span class="sxs-lookup"><span data-stu-id="35954-124">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="35954-125">لمزيد من المعلومات ، راجع [تسجيل تطبيق web app باستخدام مدخل Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span><span class="sxs-lookup"><span data-stu-id="35954-125">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="35954-126">أضف عنوان URI لأعاده التوجيه لموقع بعد نشر التطبيق في ذلك الموقع.</span><span class="sxs-lookup"><span data-stu-id="35954-126">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="35954-127">**تعذر تسجيل عناوين Url للردات كافيه**</span><span class="sxs-lookup"><span data-stu-id="35954-127">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="35954-128">أنت بائع البريد المستقل (ISV) ولديك معرفات واحده أو أكثر لأعاده توجيه البريد الخاصة بكل عميل لك.</span><span class="sxs-lookup"><span data-stu-id="35954-128">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="35954-129">تريد الترحيل من ADAL/Azure AD v 1.0 إلى مسال/النظام الأساسي لهويه Microsoft وقد وصلت إلى [الحد الأقصى لعدد uri أعاده التوجيه](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="35954-129">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="35954-130">لحل هذه المشكلة ، [أضف التوجيه uri إلى أساسيات الخدمة](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) التي تتوافق مع كل عميل.</span><span class="sxs-lookup"><span data-stu-id="35954-130">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
