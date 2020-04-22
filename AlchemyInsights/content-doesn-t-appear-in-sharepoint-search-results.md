---
title: لا يظهر المحتوى في نتائج بحث SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705648"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="ac844-102">لا يظهر المحتوى في نتائج بحث SharePoint</span><span class="sxs-lookup"><span data-stu-id="ac844-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="ac844-103">اتبع خطوات استكشاف الأخطاء وإصلاحها هذه عند عدم ظهور المحتوى المتوقع في نتائج البحث:</span><span class="sxs-lookup"><span data-stu-id="ac844-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="ac844-104">تأكد من تعيين **الموقع** الذي يحتوي على المحتوى المتوقع للسماح بالظهور في نتائج البحث.</span><span class="sxs-lookup"><span data-stu-id="ac844-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="ac844-105">اتبع الخطوات في [إظهار المحتوى على موقع في نتائج البحث](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="ac844-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="ac844-106">تأكد من تعيين **القائمة** أو **المكتبة** التي تحتوي على المحتوى المتوقع للسماح بالظهور في نتائج البحث.</span><span class="sxs-lookup"><span data-stu-id="ac844-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="ac844-107">اتبع الخطوات في [إظهار المحتوى من القوائم أو المكتبات في نتائج البحث](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="ac844-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="ac844-108">تحقق من نشر الصفحة أو المستند أو تخطيط الصفحة المخصصة **كإصدار رئيسي.**</span><span class="sxs-lookup"><span data-stu-id="ac844-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="ac844-109">اتبع الخطوة 3 في [البحث لا ترجع جميع النتائج في SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="ac844-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="ac844-110">تحقق من أن المستخدم لديه **أذونات** لعرض المحتوى.</span><span class="sxs-lookup"><span data-stu-id="ac844-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="ac844-111">اتبع الخطوات في [فهم مستويات الأذونات في SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="ac844-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="ac844-112">إذا تم تغيير مخطط البحث عن طريق إضافة خاصية مدارة جديدة، أو عن طريق تحرير خاصية مدارة، أو عن طريق إزالة خاصية مدارة، فستكون هناك حاجة إلى طلب تتبع ارتباطات وإعادة فهرس.</span><span class="sxs-lookup"><span data-stu-id="ac844-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="ac844-113">**إعادة فهرسة** المحتوى باتباع الخطوات في [طلب تتبع الارتباطات وإعادة الفهرسة موقع أو مكتبة أو قائمة يدوياً.](https://docs.microsoft.com/sharepoint/crawl-site-content)</span><span class="sxs-lookup"><span data-stu-id="ac844-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="ac844-114">قد يستغرق هذا بعض الوقت، انتظر 24 ساعة قبل التحقق من النتائج مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="ac844-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="ac844-115">لمزيد من المعلومات، راجع [تمكين المحتوى على موقع للبحث.](https://docs.microsoft.com/sharepoint/make-site-content-searchable)</span><span class="sxs-lookup"><span data-stu-id="ac844-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
