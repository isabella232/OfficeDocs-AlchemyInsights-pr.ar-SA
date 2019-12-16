---
title: البحث في SharePoint علي الإنترنت
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044030"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="0e1dc-102">تتبع ارتباطات المحتوي وفهرسته في SharePoint علي الإنترنت</span><span class="sxs-lookup"><span data-stu-id="0e1dc-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="0e1dc-103">يجب ان يتم تتبع ارتباطات المحتوي وأضافها إلى فهرس البحث للمستخدمين للعثور علي ما يبحثون عنه في SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="0e1dc-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="0e1dc-104">يتم تتبع ارتباطات المحتوي تلقائيا استنادا إلى جدول تتبع ارتباطات محدد مسبقا (لا يمكن تغيير جدول تتبع الارتباطات).</span><span class="sxs-lookup"><span data-stu-id="0e1dc-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="0e1dc-105">يلتقط متتبع الارتباطات المحتوي الذي تم تغييره منذ الزحف الأخير ويتم تحديث الفهرس.</span><span class="sxs-lookup"><span data-stu-id="0e1dc-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="0e1dc-106">للتاكد من تتبع ارتباطات المحتوي وتحديث الفهرس ، لاحظ ما يلي:</span><span class="sxs-lookup"><span data-stu-id="0e1dc-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="0e1dc-107">تاكد من ان المحتوي يمكن العثور عليه عن طريق [جعل محتوي الموقع قابلا للبحث](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="0e1dc-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="0e1dc-108">عند تغيير خاصيه مداره ، أو عند تغيير تعيين الخصائص المتتبعة والمدارة ، يجب أعاده تتبع ارتباطات الموقع قبل ان تنعكس التغييرات في فهرس البحث.</span><span class="sxs-lookup"><span data-stu-id="0e1dc-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="0e1dc-109">لأنه يتم اجراء التغييرات في مخطط البحث ، وليس إلى الموقع الفعلي ، لن يقوم متتبع الارتباطات باعاده فهرسه الموقع تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="0e1dc-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="0e1dc-110">لمزيد من المعلومات ، راجع [يدويا طلب تتبع الارتباطات وأعاده فهرسه موقع أو مكتبه أو قائمه](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="0e1dc-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="0e1dc-111">انتظر 24 ساعة علي الأقل بعد طلب الزحف يدويا وأعاده فهرسه كامله لمعرفه ما إذا كنت لا تزال تواجه مشكله ما.</span><span class="sxs-lookup"><span data-stu-id="0e1dc-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="0e1dc-112">إذا مرت أكثر من 24 ساعة منذ بدء تتبع الارتباطات وأعاده فهرسه كامله ، الرجاء تسجيل حاله دعم.</span><span class="sxs-lookup"><span data-stu-id="0e1dc-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="0e1dc-113">في كثير من الحالات ، نحن نعمل بالفعل علي حل.</span><span class="sxs-lookup"><span data-stu-id="0e1dc-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="0e1dc-114">من فضلك أعطنا 24 ساعة علي الأقل لإكمال الحل.</span><span class="sxs-lookup"><span data-stu-id="0e1dc-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0e1dc-115">إذا تم حذف موقع أو مستند (مكتبه) أو قائمه وما زال يظهر في نتائج البحث ، يجب ان يتلقى المستخدمون **خطا 404 لم يتم العثور علي ملف** عند محاولة الوصول اليه.</span><span class="sxs-lookup"><span data-stu-id="0e1dc-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="0e1dc-116">يجب تسجيل هذه المشكلة كحاله دعم لمزيد من التحقيق.</span><span class="sxs-lookup"><span data-stu-id="0e1dc-116">This issue should be logged as a support case for further investigation.</span></span> 



