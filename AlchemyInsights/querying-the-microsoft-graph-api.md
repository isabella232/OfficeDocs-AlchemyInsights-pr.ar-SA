---
title: الاستعلام عن واجهه برمجه تطبيقات Microsoft Graph
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974151"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="1828d-102">الاستعلام عن واجهه برمجه تطبيقات Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1828d-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="1828d-103">قد ينطبق هذا الموضوع أيضا علي المطورين الذين لا يزالوا يستخدمون واجهه برمجه تطبيقات Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1828d-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="1828d-104">ومع ذلك ، يوصي **بشده** باستخدام Microsoft Graph لكل الدليل والهوية وسيناريوهات أداره access.</span><span class="sxs-lookup"><span data-stu-id="1828d-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="1828d-105">**مشاكل المصادقة أو التخويل**</span><span class="sxs-lookup"><span data-stu-id="1828d-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="1828d-106">إذا تعذر علي تطبيقك **الحصول علي الرموز المميزة** للاتصال ب microsoft graph ، فاختر **المشكلة المتعلقة بالحصول علي التعليمات الخاصة بالرمز المميز للوصول (مصادقه)** microsoft Graph للحصول علي مزيد من المساعدة والدعم في هذا الموضوع.</span><span class="sxs-lookup"><span data-stu-id="1828d-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="1828d-107">إذا كان التطبيق الذي تريده **يتلقى 401 أو 403 خطا في التخويل** عند الاتصال بالرسم البياني ل microsoft ، فحدد الفئة الخاصة **بالحصول علي الأخطاء التي رفضها Access (التخويل)** للحصول علي تعليمات ودعم أكثر تحديدا في هذا الموضوع.</span><span class="sxs-lookup"><span data-stu-id="1828d-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="1828d-108">**ارغب في استخدام Microsoft Graph ، ولكن ليس عليك التاكد من مكان البدء**</span><span class="sxs-lookup"><span data-stu-id="1828d-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="1828d-109">لمعرفه المزيد حول Microsoft Graph ، راجع:</span><span class="sxs-lookup"><span data-stu-id="1828d-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="1828d-110">نظره عامه حول Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1828d-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="1828d-111">نظره عامه حول الهوية وأداره Access في Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1828d-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="1828d-112">بدء إنشاء تطبيقات Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1828d-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="1828d-113">**مستكشف الرسوم البيانية في microsoft** -اختبار واجات برمجه تطبيقات microsoft graph في نطاق المستاجر أو مستاجر العرض التوضيحي</span><span class="sxs-lookup"><span data-stu-id="1828d-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="1828d-114">**أريد استخدام Microsoft Graph ، ولكنه يدعم الدليل v 1.0 واجات برمجه التطبيقات التي احتاج اليها ؟**</span><span class="sxs-lookup"><span data-stu-id="1828d-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="1828d-115">ان Microsoft Graph هو واجهه برمجه التطبيقات الموصي بها للدليل والهوية وأداره الوصول.</span><span class="sxs-lookup"><span data-stu-id="1828d-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="1828d-116">ومع ذلك ، لا تزال هناك بعض الفجوات بين العناصر الممكنة في Azure AD Graph و Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1828d-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="1828d-117">راجع المقالات التالية التي تميز معظم الاختلافات المحدثة للمساعدة في اختيارك:</span><span class="sxs-lookup"><span data-stu-id="1828d-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="1828d-118">اختلافات أنواع الموارد بين الرسم البياني ل Azure AD و Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1828d-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="1828d-119">اختلافات الخصائص بين الرسم البياني ل Azure AD و Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1828d-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="1828d-120">اختلافات الأسلوب بين Azure AD و Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1828d-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="1828d-121">**عند الاستعلام عن عنصر *المستخدم* ، تكون العديد من خصائصه مفقوده**</span><span class="sxs-lookup"><span data-stu-id="1828d-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="1828d-122">`GET https://graph.microsoft.com/v1.0/users` تقوم فقط بإرجاع الخاصية 11 ، بما في ذلك Microsoft Graph يحدد تلقائيا مجموعه افتراضيه من خصائص *المستخدم* لإرجاعها.</span><span class="sxs-lookup"><span data-stu-id="1828d-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="1828d-123">إذا كنت بحاجه إلى خصائص *مستخدم* أخرى ، فاستخدم $select لاختيار الخصائص التي يحتاج اليها التطبيق.</span><span class="sxs-lookup"><span data-stu-id="1828d-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="1828d-124">جربه في **Microsoft Graph Explorer** أولا.</span><span class="sxs-lookup"><span data-stu-id="1828d-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="1828d-125">**بعض قيم خصائص المستخدم *فارغه* علي الرغم من انه اعلم انه تم تعيينها**</span><span class="sxs-lookup"><span data-stu-id="1828d-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="1828d-126">التوضيح الأكثر احتمالا هو انه تم منح التطبيق *ريدباسيك* .</span><span class="sxs-lookup"><span data-stu-id="1828d-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="1828d-127">يتيح هذا للتطبيق قراءه مجموعه محدوده من خصائص المستخدم ، وإرجاع كل الخصائص الأخرى كفارغه حتى إذا تم تعيينها مسبقا.</span><span class="sxs-lookup"><span data-stu-id="1828d-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="1828d-128">جرب منح *المستخدم التطبيق. أقرا كل* الأذونات بدلا من ذلك.</span><span class="sxs-lookup"><span data-stu-id="1828d-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="1828d-129">لمزيد من المعلومات ، راجع [أذونات مستخدمي Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="1828d-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="1828d-130">**أواجه مشكله في استخدام معلمات استعلام OData لتصفيه البيانات في طلباتي**</span><span class="sxs-lookup"><span data-stu-id="1828d-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="1828d-131">بينما يدعم Microsoft Graph مجموعه كبيره من معلمات الاستعلام OData ، لا يتم دعم العديد من هذه المعلمات بشكل كامل بواسطة خدمات الدليل (الموارد التي ترث من *ديريكتوريوبجيكت*) في Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1828d-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="1828d-132">تستمر القيود نفسها التي كانت موجودة في الرسم البياني في Azure AD</span><span class="sxs-lookup"><span data-stu-id="1828d-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="1828d-133">**غير معتمد**: $count و $search و $filter علي قيم *خاليه* أو *فارغه*</span><span class="sxs-lookup"><span data-stu-id="1828d-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="1828d-134">**غير معتمد**: $filter علي خصائص معينه (راجع مواضيع الموارد التي يتم قابله للتصفية الخصائص بها)</span><span class="sxs-lookup"><span data-stu-id="1828d-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="1828d-135">**غير معتمد**: الترحيل والتصفية والفرز في الوقت نفسه</span><span class="sxs-lookup"><span data-stu-id="1828d-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="1828d-136">**غير معتمد**: تصفيه علاقة.</span><span class="sxs-lookup"><span data-stu-id="1828d-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="1828d-137">علي سبيل المثال ، يمكنك العثور علي كل أعضاء المجموعة الهندسية الموجودة في المملكة المتحدة.</span><span class="sxs-lookup"><span data-stu-id="1828d-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="1828d-138">**الدعم الجزئي**: $orderby علي *المستخدم* (displayName و الوحدات التي ليست فقط) والمجموعة </span><span class="sxs-lookup"><span data-stu-id="1828d-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="1828d-139">**الدعم الجزئي**: $filter ( *يعتمد فقط* الدعم *الستارتسويث* أو الدالات الفردية *أو* المحدودة) ، وال$expand (توسيع علاقات كائن واحد ترجع كل العلاقات ، ولكن توسيع مجموعه من الكائنات التي تقتصر عليها العلاقات) </span><span class="sxs-lookup"><span data-stu-id="1828d-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="1828d-140">لمزيد من المعلومات ، راجع [تخصيص الاستجابات باستخدام معلمات الاستعلام](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1828d-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="1828d-141">**لا تعمل واجهه برمجه التطبيقات (API) التي أقوم بالاتصال بها ، حيث يمكنني اجراء المزيد من الاختبارات ؟**</span><span class="sxs-lookup"><span data-stu-id="1828d-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="1828d-142">**مستكشف Microsoft graph** -اختبر واجات برمجه تطبيقات microsoft graph في نطاق المستاجر أو مستاجر العرض التوضيحي ، وراجع أيضا **نماذج الاستعلامات** في مستكشف Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1828d-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="1828d-143">**عندما أقوم بالاستعلام عن بيانات يبدو انه تمت أعاده تعيين بيانات غير مكتملة**</span><span class="sxs-lookup"><span data-stu-id="1828d-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="1828d-144">إذا كنت تقوم بالاستعلام عن مجموعه (مثل *المستخدمين*) ، فان Microsoft Graph يستخدم حدود الصفحة من جانب الخادم حتى يتم دائما إرجاع النتائج بحجم صفحه افتراضي.</span><span class="sxs-lookup"><span data-stu-id="1828d-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="1828d-145">يجب ان يتوقع تطبيقك دائما الوصول إلى الصفحة عبر المجموعات التي يتم إرجاعها من الخدمة.</span><span class="sxs-lookup"><span data-stu-id="1828d-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="1828d-146">لمزيد من المعلومات، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="1828d-146">For more information, see:</span></span>

- [<span data-ttu-id="1828d-147">أفضل الممارسات في Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1828d-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="1828d-148">ترحيل بيانات الرسومات البيانية في Microsoft إلى التطبيق</span><span class="sxs-lookup"><span data-stu-id="1828d-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="1828d-149">**التطبيق الخاص بي بطيء جدا وهو أيضا يتم التحكم فيه. ما هي التحسينات التي يمكنني القيام بها ؟**</span><span class="sxs-lookup"><span data-stu-id="1828d-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="1828d-150">استنادا إلى السيناريو الذي تستخدمه ، هناك مجموعه متنوعة من الخيارات المختلفة عند التخلص لتطبيقك بشكل أكثر فاعليه ، وفي بعض الحالات ، اقل عرضه ليتم التحكم فيها من قبل الخدمة (عند اجراء مكالمات كثيره جدا).</span><span class="sxs-lookup"><span data-stu-id="1828d-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="1828d-151">للتعرّف على المزيد، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="1828d-151">To learn more, see:</span></span>

- [<span data-ttu-id="1828d-152">أفضل الممارسات في Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1828d-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="1828d-153">طلبات التجميع</span><span class="sxs-lookup"><span data-stu-id="1828d-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="1828d-154">تعقب التغييرات عبر استعلام دلتا</span><span class="sxs-lookup"><span data-stu-id="1828d-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="1828d-155">الحصول علي اعلام بالتغييرات عبر ويبهوكس</span><span class="sxs-lookup"><span data-stu-id="1828d-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="1828d-156">إرشادات التحكم</span><span class="sxs-lookup"><span data-stu-id="1828d-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="1828d-157">**أين يمكنني العثور علي مزيد من المعلومات حول الأخطاء والمشاكل المعروفة ؟**</span><span class="sxs-lookup"><span data-stu-id="1828d-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="1828d-158">معلومات الاستجابة لخطا Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1828d-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="1828d-159">المشاكل المعروفة في Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1828d-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="1828d-160">**أين يمكنني التحقق من حاله توفر الخدمة والاتصال ؟**</span><span class="sxs-lookup"><span data-stu-id="1828d-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="1828d-161">يمكن ان تؤثر أتاحه الخدمة والاتصال بالخدمات الاساسيه التي يمكن الوصول اليها من خلال Microsoft Graph علي التوفر والأداء الكلي ل Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1828d-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="1828d-162">بالنسبة إلى حماية خدمه Active Directory في Azure ، تحقق من حاله **الأمان + خدمات الهوية** المدرجة في [صفحه حاله Azure](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="1828d-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="1828d-163">بالنسبة إلى خدمات Office التي تساهم في Microsoft Graph ، تحقق من حاله الخدمات المدرجة في [لوحه معلومات حماية خدمه Office](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="1828d-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
