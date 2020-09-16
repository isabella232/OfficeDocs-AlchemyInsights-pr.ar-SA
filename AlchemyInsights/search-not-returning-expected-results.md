---
title: 1491-بحث-لا-إرجاع النتائج المتوقعة
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
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740461"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="1aeba-102">لا يرجع بحث المحتوي النتائج المتوقعة</span><span class="sxs-lookup"><span data-stu-id="1aeba-102">Content Search not returning expected results</span></span>

<span data-ttu-id="1aeba-103">عند تشغيل عمليات البحث عن المحتوي من مركز توافق & أمان Microsoft 365 ، قد تتلقي نتائج بحث غير متوقعه.</span><span class="sxs-lookup"><span data-stu-id="1aeba-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="1aeba-104">خذ في الاعتبار الأمور التالية التي يمكنها ان تؤثر علي نتائج البحث:</span><span class="sxs-lookup"><span data-stu-id="1aeba-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="1aeba-105">**مواقع المحتوي وشروط البحث**: تاكد من انك قمت بتحديد مواقع المحتوي المناسبة وشروط البحث.</span><span class="sxs-lookup"><span data-stu-id="1aeba-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="1aeba-106">إذا قمت بتشغيل بحث كبير (باستخدام العديد من المواقع) ، فيمكنك تقسيمها إلى عده عمليات بحث.</span><span class="sxs-lookup"><span data-stu-id="1aeba-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="1aeba-107">**العناصر المفهرسة جزئيا**: يتم تضمين  [العناصر المفهرسة جزئيا](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) من علب البريد في نتائج البحث المقدرة.</span><span class="sxs-lookup"><span data-stu-id="1aeba-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="1aeba-108">ومع ذلك ، لا يتم تضمين العناصر المفهرسة جزئيا من المواقع في SharePoint و OneDrive في تقدير البحث.</span><span class="sxs-lookup"><span data-stu-id="1aeba-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="1aeba-109">**فشل البحث**: عند البحث في عدد كبير من علب البريد (عبر علب بريد 100,000) ، قد تحصل علي أخطاء في البحث ، مع رموز الخطا مثل CS008-009 و CS012-002).</span><span class="sxs-lookup"><span data-stu-id="1aeba-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="1aeba-110">في هذه الحالة ، أعد محاولة البحث لمواقع المحتوي الفاشلة فقط.</span><span class="sxs-lookup"><span data-stu-id="1aeba-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="1aeba-111">راجع  [هذه المقالة](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="1aeba-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
