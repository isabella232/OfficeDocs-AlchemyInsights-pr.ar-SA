---
title: 1490-استكشاف الأخطاء وإصلاحها-eDiscovery-فشل
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277826"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="e6448-102">استكشاف أخطاء البحث في المحتوي وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="e6448-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="e6448-103">هل تواجه مشاكل في البحث عن المحتوي أو الحصول علي حالات الفشل عند تصدير نتائج البحث ؟</span><span class="sxs-lookup"><span data-stu-id="e6448-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="e6448-104">علي سبيل المثال ، يمكنك تلقي ما يلي عند تشغيل عمليات البحث ؟</span><span class="sxs-lookup"><span data-stu-id="e6448-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="e6448-105">أخطاء CS008 أو CS012</span><span class="sxs-lookup"><span data-stu-id="e6448-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="e6448-106">أخطاء مشغولة/مهله الخادم</span><span class="sxs-lookup"><span data-stu-id="e6448-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="e6448-107">حدث خطا في التطبيق</span><span class="sxs-lookup"><span data-stu-id="e6448-107">Application error occurred</span></span>

<span data-ttu-id="e6448-108">أو عند البحث أو التصدير من عدد كبير من علب البريد (عبر علب بريد 100,000) ، هل تحصل علي أخطاء التصدير ؟</span><span class="sxs-lookup"><span data-stu-id="e6448-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="e6448-109">بالنسبة إلى هذه الأنواع من الأخطاء ، أعد محاولة البحث عن مواقع المحتوي التي فشلت.</span><span class="sxs-lookup"><span data-stu-id="e6448-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="e6448-110">راجع  [هذه المقالة](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="e6448-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="e6448-111">إذا كنت تقوم بتصدير أكثر من 100 كيلوبايت ، ستحتاج إلى استخدام Powershell التالي لتنزيل نتائج التصدير:  [تصدير النتائج من أكثر من 100 كيلوبايت علبه بريد](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="e6448-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
