---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776069"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="77238-102">البحث عن المحتوى لا يتم إرجاع النتائج المتوقعة</span><span class="sxs-lookup"><span data-stu-id="77238-102">Content Search not returning expected results</span></span>

<span data-ttu-id="77238-103">عند تشغيل "محتوى البحث" من & Office 365 أمان مركز التوافق، قد تتلقى نتائج غير متوقعة.</span><span class="sxs-lookup"><span data-stu-id="77238-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="77238-104">خذ بعين الاعتبار الأمور التالية التي يمكن أن تؤثر على نتائج البحث:</span><span class="sxs-lookup"><span data-stu-id="77238-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="77238-105">**مواقع المحتوى وشروط البحث**: تأكد من تحديد مواقع المحتوى المناسب وشروط البحث.</span><span class="sxs-lookup"><span data-stu-id="77238-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="77238-106">إذا قمت بتشغيل بحث كبيرة (مع العديد من المواقع)، خذ بعين الاعتبار تقسيمه إلى عدة عمليات البحث.</span><span class="sxs-lookup"><span data-stu-id="77238-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="77238-107">**فهرسة العناصر جزئيا**: [فهرسة العناصر جزئيا](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) من علب بريد المضمنة في نتائج البحث المقدر.</span><span class="sxs-lookup"><span data-stu-id="77238-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="77238-108">ومع ذلك، لا يتم تضمين العناصر المفهرسة جزئيا من مواقع SharePoint وأندريف في تقدير البحث.</span><span class="sxs-lookup"><span data-stu-id="77238-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="77238-109">**فشل البحث**: عند البحث في عدد كبير من علب البريد (أكثر من 000 100 علب البريد)، قد تتلقى أخطاء البحث، مع رموز الخطأ مثل CS008 009 و CS012-002).</span><span class="sxs-lookup"><span data-stu-id="77238-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="77238-110">في هذه الحالة، أعد محاولة البحث عن مواقع المحتوى الفاشلة فقط.</span><span class="sxs-lookup"><span data-stu-id="77238-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="77238-111">راجع [هذه المقالة](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="77238-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
