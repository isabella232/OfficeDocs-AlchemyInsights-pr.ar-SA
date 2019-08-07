---
title: البحث في SharePoint على الإنترنت
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: fc49978fbd2c07381dae83061b1a1868cd1df0d0
ms.sourcegitcommit: 327a2c77afc2ff3d67d3aaaea1a92068a3c4bb1f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/06/2019
ms.locfileid: "36059239"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="b0e65-102">البحث في SharePoint على الإنترنت</span><span class="sxs-lookup"><span data-stu-id="b0e65-102">Search in SharePoint Online</span></span>

<span data-ttu-id="b0e65-103">يجب أن تتبع ارتباطات المحتوى وإضافتها إلى فهرس البحث للمستخدمين للبحث عن ما كانت تبحث عنه في SharePoint على الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="b0e65-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="b0e65-104">يتم تلقائياً تتبع ارتباطات المحتوى بناء على جدول تتبع ارتباطات معرف مسبقاً (لا يمكن تغيير جدول تتبع ارتباطات).</span><span class="sxs-lookup"><span data-stu-id="b0e65-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="b0e65-105">يلتقط متتبع الارتباطات المحتوى الذي قد تغير منذ آخر عملية تتبع الارتباطات وتحديث الفهرس.</span><span class="sxs-lookup"><span data-stu-id="b0e65-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="b0e65-106">للتأكد من تتبع ارتباطات المحتوى وتحديث الفهرس، لاحظ ما يلي:</span><span class="sxs-lookup"><span data-stu-id="b0e65-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="b0e65-107">تأكد من أن المحتوى يمكن العثور عليها [جعل محتوى الموقع للبحث](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="b0e65-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="b0e65-108">عندما قمت بتغيير خاصية مدارة، أو عندما قمت بتغيير التعيين التي تم تتبع ارتباطاتها وإدارتها يجب إعادة المتتبعة خصائص الموقع قبل سوف تنعكس التغييرات في فهرس البحث.</span><span class="sxs-lookup"><span data-stu-id="b0e65-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="b0e65-109">لأنه يتم إجراء التغييرات في مخطط البحث، ولا إلى الموقع الفعلي، متتبع الارتباطات سيتم تلقائياً إعادة فهرسة الموقع.</span><span class="sxs-lookup"><span data-stu-id="b0e65-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="b0e65-110">لمزيد من المعلومات، راجع [طلب تتبع الارتباطات وإعادة فهرسة موقع أو مكتبة أو قائمة يدوياً](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="b0e65-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="b0e65-111">انتظر 24 ساعة على الأقل بعد طلب تتبع الارتباطات والكامل إعادة الفهرسة لمعرفة إذا كنت لا تزال تواجه مشكلة يدوياً.</span><span class="sxs-lookup"><span data-stu-id="b0e65-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="b0e65-112">في حالة مرور أكثر من 24 ساعة منذ بدء تتبع الارتباطات والكامل إعادة الفهرسة، الرجاء تسجيل حالة دعم.</span><span class="sxs-lookup"><span data-stu-id="b0e65-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="b0e65-113">في كثير من الحالات، الفعل نعمل على إيجاد حل.</span><span class="sxs-lookup"><span data-stu-id="b0e65-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b0e65-114">الرجاء إعطاء لنا أربع وعشرين ساعة لإكمال حل.</span><span class="sxs-lookup"><span data-stu-id="b0e65-114">Please give us at least 24 hours to complete a solution.</span></span>

>[! هام!]<span data-ttu-id="b0e65-115">: إذا كان موقع المستند (مكتبة) أو قائمة محذوف ولا يزال يظهر في نتائج البحث، يجب أن يتلقى المستخدمون **الخطأ 404 تعذر العثور على ملف** عند محاولة الوصول إليه.</span><span class="sxs-lookup"><span data-stu-id="b0e65-115">: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="b0e65-116">يجب تسجيل هذه المشكلة كحالة دعم لإجراء مزيد من التحقيقات.</span><span class="sxs-lookup"><span data-stu-id="b0e65-116">This issue should be logged as a support case for further investigation.</span></span> 



