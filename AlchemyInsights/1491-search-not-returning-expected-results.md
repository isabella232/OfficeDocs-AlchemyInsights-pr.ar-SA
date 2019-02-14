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
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964791"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="1909f-102">البحث عن المحتوى لا يتم إرجاع النتائج المتوقعة</span><span class="sxs-lookup"><span data-stu-id="1909f-102">Content Search not returning expected results</span></span>

<span data-ttu-id="1909f-p101">عند تشغيل "محتوى البحث" من & Office 365 أمان مركز التوافق، قد تتلقى نتائج غير متوقعة. خذ بعين الاعتبار الأمور التالية التي يمكن أن تؤثر على نتائج البحث:</span><span class="sxs-lookup"><span data-stu-id="1909f-p101">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results. Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="1909f-p102">**مواقع المحتوى وشروط البحث**: تأكد من تحديد مواقع المحتوى المناسب وشروط البحث. إذا قمت بتشغيل بحث كبيرة (مع العديد من المواقع)، خذ بعين الاعتبار تقسيمه إلى عدة عمليات البحث.</span><span class="sxs-lookup"><span data-stu-id="1909f-p102">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions. If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="1909f-p103">**فهرسة العناصر جزئيا**: [فهرسة العناصر جزئيا](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) من علب بريد المضمنة في نتائج البحث المقدر. ومع ذلك، لا يتم تضمين العناصر المفهرسة جزئيا من مواقع SharePoint وأندريف في تقدير البحث.</span><span class="sxs-lookup"><span data-stu-id="1909f-p103">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results. However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="1909f-p104">**فشل البحث**: عند البحث في عدد كبير من علب البريد (أكثر من 000 100 علب البريد)، قد تتلقى أخطاء البحث، مع رموز الخطأ مثل CS008 009 و CS012-002). في هذه الحالة، أعد محاولة البحث عن مواقع المحتوى الفاشلة فقط. راجع [هذه المقالة](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="1909f-p104">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002). In this case, retry the search only for the failed content locations. See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
