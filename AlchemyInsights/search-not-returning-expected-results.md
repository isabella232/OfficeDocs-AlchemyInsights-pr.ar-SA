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
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 094da9d75013aae56ca219b7ae03e85736ce5ee0
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551402"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="c2e5e-102">البحث عن المحتوى لا يتم إرجاع النتائج المتوقعة</span><span class="sxs-lookup"><span data-stu-id="c2e5e-102">Content Search not returning expected results</span></span>

<span data-ttu-id="c2e5e-103">عند تشغيل "محتوى البحث" من & Office 365 أمان مركز التوافق، قد تتلقى نتائج غير متوقعة.</span><span class="sxs-lookup"><span data-stu-id="c2e5e-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="c2e5e-104">خذ بعين الاعتبار الأمور التالية التي يمكن أن تؤثر على نتائج البحث:</span><span class="sxs-lookup"><span data-stu-id="c2e5e-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="c2e5e-105">**مواقع المحتوى وشروط البحث**: تأكد من تحديد مواقع المحتوى المناسب وشروط البحث.</span><span class="sxs-lookup"><span data-stu-id="c2e5e-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="c2e5e-106">إذا قمت بتشغيل بحث كبيرة (مع العديد من المواقع)، خذ بعين الاعتبار تقسيمه إلى عدة عمليات البحث.</span><span class="sxs-lookup"><span data-stu-id="c2e5e-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="c2e5e-107">**فهرسة العناصر جزئيا**: [فهرسة العناصر جزئيا](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) من علب بريد المضمنة في نتائج البحث المقدر.</span><span class="sxs-lookup"><span data-stu-id="c2e5e-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="c2e5e-108">ومع ذلك، لا يتم تضمين العناصر المفهرسة جزئيا من مواقع SharePoint وأندريف في تقدير البحث.</span><span class="sxs-lookup"><span data-stu-id="c2e5e-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="c2e5e-109">**فشل البحث**: عند البحث في عدد كبير من علب البريد (أكثر من 000 100 علب البريد)، قد تتلقى أخطاء البحث، مع رموز الخطأ مثل CS008 009 و CS012-002).</span><span class="sxs-lookup"><span data-stu-id="c2e5e-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="c2e5e-110">في هذه الحالة، أعد محاولة البحث عن مواقع المحتوى الفاشلة فقط.</span><span class="sxs-lookup"><span data-stu-id="c2e5e-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="c2e5e-111">راجع [هذه المقالة](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="c2e5e-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
