---
title: البحث في SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f790efbe6ed445786933efa3fc980f974693d1d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770754"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="6f88a-102">تتبع ارتباطات المحتوي والفهرسة في SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6f88a-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="6f88a-103">يجب ان يتم تتبع ارتباطات المحتوي وأضافه إلى فهرس البحث للمستخدمين للعثور علي ما يبحثون عنه في SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="6f88a-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span>

- <span data-ttu-id="6f88a-104">تاكد من انه يمكن العثور علي المحتوي من خلال [تمكين البحث في محتوي الموقع](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="6f88a-104">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="6f88a-105">عند تغيير الخاصية المدارة ، أو عند تغيير تخطيط الخصائص التي تم تتبع ارتباطاتها وأدارتها ، يجب أعاده تتبع ارتباطات الموقع قبل ان تنعكس تغييراتك في فهرس البحث.</span><span class="sxs-lookup"><span data-stu-id="6f88a-105">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span>

- <span data-ttu-id="6f88a-106">لمزيد من المعلومات ، راجع [طلب التسجيل التلقائي لتتبع الارتباطات وأعاده فهرسه موقع أو مكتبه أو قائمه](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="6f88a-106">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span>

- <span data-ttu-id="6f88a-107">انتظر 24 ساعة علي الأقل بعد طلب عمليه تتبع الارتباطات وأعاده الفهرسة بالبالكامل لمعرفه ما إذا كنت لا تزال تواجه مشكله.</span><span class="sxs-lookup"><span data-stu-id="6f88a-107">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span>

- <span data-ttu-id="6f88a-108">إذا تم تمرير أكثر من 24 ساعة منذ ان قمت ببدء عمليه تتبع الارتباطات وأعاده الفهرسة بالبالكامل ، فيرجى تسجيل حاله دعم.</span><span class="sxs-lookup"><span data-stu-id="6f88a-108">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="6f88a-109">في حالات كثيره ، نحن نعمل بالفعل علي حل.</span><span class="sxs-lookup"><span data-stu-id="6f88a-109">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="6f88a-110">يرجى تقديم 24 ساعة علي الأقل لإكمال حل.</span><span class="sxs-lookup"><span data-stu-id="6f88a-110">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="6f88a-111">**هام**: إذا تم حذف موقع أو مستند (مكتبه) أو قائمه وكانت لا تزال تظهر في نتائج البحث ، فيجب ان يتلقى المستخدمون **ملف خطا 404 لم يتم العثور عليه** عند محاولة الوصول اليه.</span><span class="sxs-lookup"><span data-stu-id="6f88a-111">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="6f88a-112">يجب ان يتم تسجيل هذه المشكلة كحاله دعم لمزيد من الاستقصاء.</span><span class="sxs-lookup"><span data-stu-id="6f88a-112">This issue should be logged as a support case for further investigation.</span></span>



