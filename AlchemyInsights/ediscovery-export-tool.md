---
title: أداة تصدير eDiscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814575"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="be770-102">هل لا يمكنك تثبيت أداة تصدير eDiscovery أو تشغيلها؟</span><span class="sxs-lookup"><span data-stu-id="be770-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="be770-103">إذا لم تتمكن من تثبيت أداة تصدير eDiscovery أو تشغيلها لتنزيل نتائج البحث، فتحقق من الأمور التالية:</span><span class="sxs-lookup"><span data-stu-id="be770-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="be770-104">يلبي الكمبيوتر الذي تستخدمه هذه المتطلبات الأساسية:</span><span class="sxs-lookup"><span data-stu-id="be770-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="be770-105">الإصدارات 32- أو 64 بت من Windows 7 والإصدارات الأحدث</span><span class="sxs-lookup"><span data-stu-id="be770-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="be770-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="be770-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="be770-107">مستعرض معتمد:</span><span class="sxs-lookup"><span data-stu-id="be770-107">A supported browser:</span></span>

  - <span data-ttu-id="be770-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="be770-108">Microsoft Edge</span></span>

    <span data-ttu-id="be770-109">أو</span><span class="sxs-lookup"><span data-stu-id="be770-109">Or</span></span>

  - <span data-ttu-id="be770-110">Internet Explorer 10 والإصدارات الأحدث</span><span class="sxs-lookup"><span data-stu-id="be770-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="be770-111">المستعرضات الأخرى، مثل Google Chrome و Mozilla Firefox غير معتمدة.</span><span class="sxs-lookup"><span data-stu-id="be770-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="be770-112">يمكن لمنظمتك الاتصال بنقطة النهاية في Azure، **\* وهي .blob.core.windows.net** (يمثل أحرف البدل معرفا فريدا لمهمة التصدير).</span><span class="sxs-lookup"><span data-stu-id="be770-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="be770-113">تم تعيين دور التصدير في مركز التوافق الأمني ل Microsoft 365. &amp;</span><span class="sxs-lookup"><span data-stu-id="be770-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="be770-114">بشكل افتراضي، يتم تعيين هذا الدور إلى مجموعة دور eDiscovery Manager فقط.</span><span class="sxs-lookup"><span data-stu-id="be770-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="be770-115">راجع [تعيين أذونات eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="be770-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="be770-116">لمزيد من المعلومات، راجع [تصدير نتائج البحث في المحتوى](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="be770-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="be770-117">إذا كنت تقوم بتصدير أكثر من 100 ألف علبة بريد، ستحتاج إلى استخدام Powershell التالي لتنزيل نتائج التصدير: تصدير النتائج من أكثر من  [100 ألف](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)علبة بريد .</span><span class="sxs-lookup"><span data-stu-id="be770-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>