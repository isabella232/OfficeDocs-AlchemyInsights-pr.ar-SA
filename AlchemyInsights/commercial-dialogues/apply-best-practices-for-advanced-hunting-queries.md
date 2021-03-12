---
title: تطبيق أفضل الممارسات لاستعلامات الصيد المتقدمة
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743120"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="1e4ab-102">تطبيق أفضل الممارسات لاستعلامات الصيد المتقدمة</span><span class="sxs-lookup"><span data-stu-id="1e4ab-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="1e4ab-103">للحصول على النتائج بشكل أسرع وتجنب المهات أثناء تشغيل الاستعلامات المعقدة، طبق أفضل الممارسات التالية:</span><span class="sxs-lookup"><span data-stu-id="1e4ab-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="1e4ab-104">عند تجربة استعلامات جديدة، استخدم دائما حد لتجنب الحصول على مجموعات نتائج كبيرة جدا.</span><span class="sxs-lookup"><span data-stu-id="1e4ab-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="1e4ab-105">أيضا، استخدم هذا التقييم لتقييم أولي لحجم `count` مجموعة النتائج.</span><span class="sxs-lookup"><span data-stu-id="1e4ab-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="1e4ab-106">استخدم عوامل تصفية الوقت أولا.</span><span class="sxs-lookup"><span data-stu-id="1e4ab-106">Use time filters first.</span></span> <span data-ttu-id="1e4ab-107">وبشكل مثالي، حصر الاستعلامات بسبعة أيام.</span><span class="sxs-lookup"><span data-stu-id="1e4ab-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="1e4ab-108">في بداية استعلام، بعد عامل تصفية الوقت مباشرة، أضف عوامل التصفية المتوقعة لإزالة معظم البيانات.</span><span class="sxs-lookup"><span data-stu-id="1e4ab-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="1e4ab-109">عند البحث عن الرموز المميزة الكاملة، استخدم `has` عامل التشغيل بدلا من `contains` .</span><span class="sxs-lookup"><span data-stu-id="1e4ab-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="1e4ab-110">يمكنك تشغيل عملية بحث على عمود معين بدلا من تشغيلها عبر كل الأعمدة.</span><span class="sxs-lookup"><span data-stu-id="1e4ab-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="1e4ab-111">عند الانضمام إلى الجداول، حدد الجدول الذي به صفوف أقل أولا.</span><span class="sxs-lookup"><span data-stu-id="1e4ab-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="1e4ab-112">`project` الأعمدة الضرورية فقط من الجداول التي قمت بضمها.</span><span class="sxs-lookup"><span data-stu-id="1e4ab-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="1e4ab-113">لمعرفة المزيد، راجع [أفضل ممارسات استعلام البحث المتقدم](https://go.microsoft.com/fwlink/?linkid=2144812).</span><span class="sxs-lookup"><span data-stu-id="1e4ab-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
