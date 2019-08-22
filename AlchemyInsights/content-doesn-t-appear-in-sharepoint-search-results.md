---
title: لا يظهر المحتوى في نتائج البحث SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ffb6bf349f9e8c2323186a8fc3183325d1d7e1bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517018"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="b8fa3-102">لا يظهر المحتوى في نتائج البحث SharePoint</span><span class="sxs-lookup"><span data-stu-id="b8fa3-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="b8fa3-103">اتبع خطوات استكشاف الأخطاء وإصلاحها عندما لا يظهر المحتوى المتوقع في نتائج البحث:</span><span class="sxs-lookup"><span data-stu-id="b8fa3-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="b8fa3-104">تحقق من أن يتم تعيين **الموقع** الذي يحتوي على المحتوى المتوقع السماح بالمحتوى التي تظهر في نتائج البحث.</span><span class="sxs-lookup"><span data-stu-id="b8fa3-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="b8fa3-105">اتبع الخطوات الموجودة في [إظهار المحتوى على موقع في نتائج البحث](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="b8fa3-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="b8fa3-106">تحقق من تعيين **القائمة** أو **المكتبة** التي تحتوي على المحتوى المتوقع السماح بالمحتوى التي تظهر في نتائج البحث.</span><span class="sxs-lookup"><span data-stu-id="b8fa3-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="b8fa3-107">اتبع الخطوات الموجودة في [إظهار المحتوى من القوائم أو المكتبات الموجودة في نتائج البحث](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="b8fa3-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="b8fa3-108">التحقق من نشر الصفحة أو المستند، أو تخطيط الصفحة المخصصة **الإصدار الرئيسي.**</span><span class="sxs-lookup"><span data-stu-id="b8fa3-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="b8fa3-109">اتبع الخطوة رقم 3 في [البحث لا ترجع كافة النتائج في SharePoint على الإنترنت](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="b8fa3-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="b8fa3-110">تحقق من أن المستخدم لديه **أذونات** لعرض المحتوى.</span><span class="sxs-lookup"><span data-stu-id="b8fa3-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="b8fa3-111">اتبع الخطوات الموجودة في [فهم "مستويات الإذن" في SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="b8fa3-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="b8fa3-112">إذا تم تغيير مخطط البحث بإضافة خاصية جديدة مدارة أو عن طريق تحرير خاصية مدارة أو عن طريق إزالة خاصية مدارة ثم يطلب منه عملية تتبع ارتباطات وسيكون مطلوباً إعادة الفهرسة.</span><span class="sxs-lookup"><span data-stu-id="b8fa3-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="b8fa3-113">**إعادة فهرسة** المحتوى باتباع الخطوات المذكورة في [طلب يدوياً تتبع الارتباطات وإعادة فهرسة موقع أو قائمة أو مكتبة](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="b8fa3-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="b8fa3-114">وهذا قد يستغرق بعض الوقت، الانتظار 24 ساعة قبل التحقق من النتائج.</span><span class="sxs-lookup"><span data-stu-id="b8fa3-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="b8fa3-115">لمزيد من المعلومات، راجع [تمكين المحتوى على موقع يمكن البحث فيها](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="b8fa3-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
