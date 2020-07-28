---
title: يعرض المخطط عددًا مختلفًا من السجلات في الشبكة
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438695"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="03200-102">يعرض المخطط عددًا مختلفًا من السجلات في الشبكة</span><span class="sxs-lookup"><span data-stu-id="03200-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="03200-103">**اعراض**</span><span class="sxs-lookup"><span data-stu-id="03200-103">**Symptom**</span></span>

<span data-ttu-id="03200-104">بالنسبة للمخطط في صفحة لوحة المعلومات، عند النقر على المخطط "..." وانقر على "عرض السجلات"، انتقل إلى صفحة الشبكة لمشاهدة كافة السجلات. في بعض الأحيان، يتغير عدد السجلات.</span><span class="sxs-lookup"><span data-stu-id="03200-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="03200-105">**يسبب**</span><span class="sxs-lookup"><span data-stu-id="03200-105">**Cause**</span></span>

<span data-ttu-id="03200-106">ويرجع ذلك إلى اختلاف طرق العرض بين المخطط على صفحة لوحة المعلومات الأصلية والمخطط على الصفحة الرئيسية للشبكة.</span><span class="sxs-lookup"><span data-stu-id="03200-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="03200-107">**حل**</span><span class="sxs-lookup"><span data-stu-id="03200-107">**Solution**</span></span>

1. <span data-ttu-id="03200-108">تحقق من طريقة العرض من الصفحة الأصلية و طريقة العرض في الشبكة لمعرفة ما إذا كانت مختلفة.</span><span class="sxs-lookup"><span data-stu-id="03200-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="03200-109">تغيير طريقة العرض في الشبكة لمطابقة طريقة العرض في الصفحة الأصلية.</span><span class="sxs-lookup"><span data-stu-id="03200-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="03200-110">إذا تعذر العثور على طريقة العرض الصحيحة، فهذا يعني عادةً أن طريقة العرض غير ممكّنة في مصمم التطبيق.</span><span class="sxs-lookup"><span data-stu-id="03200-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="03200-111">انتقل إلى مصمم التطبيق الخاص بالتطبيق المحدد، واختر الكيان وطرق عرضه، وتحقق من طريقة العرض التي تريد تمكينها، وحفظها، ونشرها وإغلاقها.</span><span class="sxs-lookup"><span data-stu-id="03200-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="03200-112">قم بتحديث الصفحة.</span><span class="sxs-lookup"><span data-stu-id="03200-112">Refresh the page.</span></span>