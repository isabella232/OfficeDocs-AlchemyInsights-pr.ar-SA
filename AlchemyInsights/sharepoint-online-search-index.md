---
title: إدارة القواميس البحث في SharePoint عبر إنترنت
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 5319c2f1edc3e61074301f039736d2aa96bda47b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758752"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="69dd9-102">البحث في SharePoint على الإنترنت</span><span class="sxs-lookup"><span data-stu-id="69dd9-102">Search in SharePoint Online</span></span>

<span data-ttu-id="69dd9-103">يجب أن تتبع ارتباطات المحتوى وإضافتها إلى فهرس البحث للمستخدمين للبحث عن ما كانت تبحث عنه في SharePoint على الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="69dd9-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="69dd9-104">يتم تلقائياً تتبع ارتباطات المحتوى بناء على جدول تتبع ارتباطات معرف مسبقاً (لا يمكن تغيير جدول تتبع ارتباطات).</span><span class="sxs-lookup"><span data-stu-id="69dd9-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="69dd9-105">يلتقط متتبع الارتباطات المحتوى الذي قد تغير منذ آخر عملية تتبع الارتباطات وتحديث الفهرس.</span><span class="sxs-lookup"><span data-stu-id="69dd9-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="69dd9-106">للتأكد من تتبع ارتباطات المحتوى وتحديث الفهرس، اتبع الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="69dd9-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="69dd9-107">تأكد من أن المحتوى يمكن العثور عليها بجعل محتوى الموقع للبحث.</span><span class="sxs-lookup"><span data-stu-id="69dd9-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="69dd9-108">لمزيد من المعلومات، راجع [تمكين المحتوى على موقع يمكن البحث فيها](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="69dd9-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="69dd9-109">عندما قمت بتغيير خاصية مدارة، أو عندما قمت بتغيير التعيين التي تم تتبع ارتباطاتها وإدارتها يجب إعادة المتتبعة خصائص الموقع قبل سوف تنعكس التغييرات في فهرس البحث.</span><span class="sxs-lookup"><span data-stu-id="69dd9-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="69dd9-110">لأنه يتم إجراء التغييرات في مخطط البحث، ولا إلى الموقع الفعلي، متتبع الارتباطات سيتم تلقائياً إعادة فهرسة الموقع.</span><span class="sxs-lookup"><span data-stu-id="69dd9-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="69dd9-111">لمزيد من المعلومات، راجع [طلب تتبع الارتباطات وإعادة فهرسة موقع أو مكتبة أو قائمة يدوياً](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="69dd9-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="69dd9-112">انتظر 24 ساعة على الأقل بعد طلب تتبع الارتباطات والكامل إعادة الفهرسة لمعرفة إذا كنت لا تزال تواجه مشكلة يدوياً.</span><span class="sxs-lookup"><span data-stu-id="69dd9-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="69dd9-113">في حالة مرور أكثر من 24 ساعة منذ بدء تتبع الارتباطات والكامل إعادة الفهرسة، الرجاء تسجيل حالة دعم.</span><span class="sxs-lookup"><span data-stu-id="69dd9-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="69dd9-114">في كثير من الحالات، الفعل نعمل على إيجاد حل.</span><span class="sxs-lookup"><span data-stu-id="69dd9-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="69dd9-115">الرجاء إعطاء لنا أربع وعشرين ساعة لإكمال حل.</span><span class="sxs-lookup"><span data-stu-id="69dd9-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="69dd9-116">**هام**: إذا كان موقع المستند (مكتبة) أو قائمة محذوف ولا يزال يظهر في نتائج البحث، يجب أن يتلقى المستخدمون "الخطأ 404 تعذر العثور على ملف" عند محاولة الوصول إلى.</span><span class="sxs-lookup"><span data-stu-id="69dd9-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="69dd9-117">يجب تسجيل هذه المشكلة كحالة دعم لإجراء مزيد من التحقيقات.</span><span class="sxs-lookup"><span data-stu-id="69dd9-117">This issue should be logged as a support case for further investigation.</span></span> 



