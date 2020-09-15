---
title: لا يظهر المحتوي في نتائج البحث في SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713117"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="5cc6c-102">لا يظهر المحتوي في نتائج البحث في SharePoint</span><span class="sxs-lookup"><span data-stu-id="5cc6c-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="5cc6c-103">اتبع خطوات استكشاف الأخطاء وإصلاحها عند عدم ظهور المحتوي المتوقع في نتائج البحث:</span><span class="sxs-lookup"><span data-stu-id="5cc6c-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="5cc6c-104">تاكد من ان **الموقع** الذي يحتوي علي المحتوي المتوقع تم تعيينه للسماح بظهور المحتوي في نتائج البحث.</span><span class="sxs-lookup"><span data-stu-id="5cc6c-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="5cc6c-105">اتبع الخطوات [الواردة في إظهار المحتوي علي موقع في نتائج البحث](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="5cc6c-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="5cc6c-106">تاكد من ان **القائمة** أو **المكتبة** التي تحتوي علي المحتوي المتوقع تم تعيينها للسماح بظهور المحتوي في نتائج البحث.</span><span class="sxs-lookup"><span data-stu-id="5cc6c-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="5cc6c-107">اتبع الخطوات الواردة في [إظهار المحتوي من القوائم أو المكتبات في نتائج البحث](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="5cc6c-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="5cc6c-108">تاكد من نشر الصفحة أو المستند أو تخطيط الصفحة المخصص **كاصدار رئيسي.**</span><span class="sxs-lookup"><span data-stu-id="5cc6c-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="5cc6c-109">اتبع الخطوة 3 في [البحث لا يتم إرجاع كل النتائج في SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="5cc6c-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="5cc6c-110">تاكد من ان المستخدم يملك **أذونات** لعرض المحتوي.</span><span class="sxs-lookup"><span data-stu-id="5cc6c-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="5cc6c-111">اتبع الخطوات الواردة في [التعرف علي مستويات الأذونات في SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="5cc6c-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="5cc6c-112">إذا تم تغيير مخطط البحث عن طريق أضافه خاصيه مداره جديده ، وذلك بتحرير خاصيه مداره ، أو بازاله خاصيه مداره ، سيطلب منك تتبع الارتباطات وأعاده الفهرسة.</span><span class="sxs-lookup"><span data-stu-id="5cc6c-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="5cc6c-113">يمكنك **أعاده فهرسه** المحتوي باتباع الخطوات الواردة في [طلب التتبع اليدوي وأعاده فهرسه موقع أو مكتبه أو قائمه](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="5cc6c-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="5cc6c-114">قد يستغرق ذلك بعض الوقت ، انتظر 24 ساعة قبل التحقق من النتائج مره أخرى.</span><span class="sxs-lookup"><span data-stu-id="5cc6c-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="5cc6c-115">لمزيد من المعلومات ، راجع [تمكين المحتوي علي موقع ليكون قابلا للبحث](https://docs.microsoft.com/sharepoint/make-site-content-searchable)فيه.</span><span class="sxs-lookup"><span data-stu-id="5cc6c-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
