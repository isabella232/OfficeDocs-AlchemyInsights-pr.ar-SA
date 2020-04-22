---
title: 1491-البحث-لا إرجاع-المتوقع-النتائج
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709214"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="91114-102">البحث عن المحتوى لا إرجاع النتائج المتوقعة</span><span class="sxs-lookup"><span data-stu-id="91114-102">Content Search not returning expected results</span></span>

<span data-ttu-id="91114-103">عند تشغيل عمليات البحث عن المحتوى من مركز التوافق & أمان Microsoft 365، قد تتلقى نتائج بحث غير متوقعة.</span><span class="sxs-lookup"><span data-stu-id="91114-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="91114-104">ضع في اعتبارك الأشياء التالية التي يمكن أن تؤثر على نتائج البحث:</span><span class="sxs-lookup"><span data-stu-id="91114-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="91114-105">**مواقع المحتوى وظروف البحث:** تأكد من تحديد مواقع المحتوى المناسبة وظروف البحث.</span><span class="sxs-lookup"><span data-stu-id="91114-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="91114-106">إذا قمت بتشغيل بحث كبير (مع العديد من المواقع)، ففكر في تقسيمه إلى عمليات بحث متعددة.</span><span class="sxs-lookup"><span data-stu-id="91114-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="91114-107">**العناصر المفهرسة جزئيًا:** يتم تضمين [العناصر المفهرسة جزئيًا](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) من علب البريد في نتائج البحث المقدرة.</span><span class="sxs-lookup"><span data-stu-id="91114-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="91114-108">ومع ذلك، لا يتم تضمين العناصر المفهرسة جزئيًا من المواقع في SharePoint و OneDrive في تقدير البحث.</span><span class="sxs-lookup"><span data-stu-id="91114-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="91114-109">**فشل البحث:** عند البحث في عدد كبير من علب البريد (أكثر من 100,000 علب ة بريد)، قد تحصل على أخطاء البحث، مع رموز الخطأ مثل CS008-009 و CS012-002).</span><span class="sxs-lookup"><span data-stu-id="91114-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="91114-110">في هذه الحالة، إعادة محاولة البحث فقط عن مواقع المحتوى الفاشلة.</span><span class="sxs-lookup"><span data-stu-id="91114-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="91114-111">راجع [هذه المقالة](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) لمزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="91114-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
