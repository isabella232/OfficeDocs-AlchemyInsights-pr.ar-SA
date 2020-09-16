---
title: أداره مخطط البحث في SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770538"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="96ebb-102">أداره مخطط البحث في SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="96ebb-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="96ebb-103">يتحكم مخطط البحث بما يمكن للمستخدمين البحث عنه ، وكيف يمكن للمستخدمين البحث عنه ، وكيفيه تقديم النتائج علي مواقع البحث علي الويب.</span><span class="sxs-lookup"><span data-stu-id="96ebb-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="96ebb-104">راجع [أداره مخطط البحث في SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) للتعرف علي كيفيه القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="96ebb-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="96ebb-105">تغيير مخطط البحث.</span><span class="sxs-lookup"><span data-stu-id="96ebb-105">Change the search schema.</span></span>
- <span data-ttu-id="96ebb-106">إنشاء الخصائص المدارة.</span><span class="sxs-lookup"><span data-stu-id="96ebb-106">Create managed properties.</span></span>
- <span data-ttu-id="96ebb-107">تعيين الخصائص المتتبعة والتي تم تتبع ارتباطاتها إلى الخصائص المدارة.</span><span class="sxs-lookup"><span data-stu-id="96ebb-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="96ebb-108">لاحظ ما يلي فيما يتعلق باداره مخطط البحث:</span><span class="sxs-lookup"><span data-stu-id="96ebb-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="96ebb-109">إذا تلقيت تحذيرا يفيد **بان التطبيق متوقف مؤقتا** عند اجراء تغيير في المخطط ، فهذا مؤقت فقط بالشكل الذي تحدث فيه صيانة الخدمة.</span><span class="sxs-lookup"><span data-stu-id="96ebb-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="96ebb-110">إذا تم تمرير أكثر من 24 ساعة وما زلت تواجه التحذير ، يرجى تسجيل حاله الدعم.</span><span class="sxs-lookup"><span data-stu-id="96ebb-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="96ebb-111">عند تغيير الخصائص المدارة أو أضافه عناصر جديده ، تصبح التغييرات ساريه المفعول فقط بعد أعاده تتبع الارتباطات للمحتوي.</span><span class="sxs-lookup"><span data-stu-id="96ebb-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="96ebb-112">في SharePoint Online ، تتم عمليه تتبع الارتباطات تلقائيا استنادا إلى جدول تتبع الارتباطات المحدد.</span><span class="sxs-lookup"><span data-stu-id="96ebb-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="96ebb-113">للتاكد من اجراء التغييرات التي تم تتبع ارتباطاتها ، يمكنك [طلب أعاده فهرسه القائمة أو المكتبة بشكل](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) خاص</span><span class="sxs-lookup"><span data-stu-id="96ebb-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="96ebb-114">للحصول علي نظره عامه حول مخطط البحث ، راجع [تقديم مخطط البحث](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="96ebb-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


