---
title: يعرض المخطط عددا مختلفا من السجلات في الشبكة
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: e499a439e7cf7e9ecbb6566f9f089f3b7b82f48e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793745"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="81028-102">يعرض المخطط عددا مختلفا من السجلات في الشبكة</span><span class="sxs-lookup"><span data-stu-id="81028-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="81028-103">**عرض**</span><span class="sxs-lookup"><span data-stu-id="81028-103">**Symptom**</span></span>

<span data-ttu-id="81028-104">بالنسبة إلى المخطط علي صفحه لوحه المعلومات ، عند النقر فوق المخطط "..." وانقر فوق "عرض السجلات" ، ثم انتقل إلى صفحه الشبكة لعرض كل السجلات. في بعض الأحيان ، يتغير عدد السجلات.</span><span class="sxs-lookup"><span data-stu-id="81028-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="81028-105">**إظهار**</span><span class="sxs-lookup"><span data-stu-id="81028-105">**Cause**</span></span>

<span data-ttu-id="81028-106">هذا ناتج عن اختلاف طرق العرض بين المخطط علي صفحه لوحه المعلومات الاصليه والمخطط علي الصفحة الرئيسية للشبكة.</span><span class="sxs-lookup"><span data-stu-id="81028-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="81028-107">**Solution**</span><span class="sxs-lookup"><span data-stu-id="81028-107">**Solution**</span></span>

1. <span data-ttu-id="81028-108">حدد طريقه العرض من الصفحة الاصليه وطريقه العرض في الشبكة لمعرفه ما إذا كانت مختلفه.</span><span class="sxs-lookup"><span data-stu-id="81028-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="81028-109">يمكنك تغيير طريقه العرض في الشبكة لمطابقه طريقه العرض في الصفحة الاصليه.</span><span class="sxs-lookup"><span data-stu-id="81028-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="81028-110">إذا تعذر العثور علي طريقه العرض الصحيحة ، فهذا يعني انه لا يتم تمكين طريقه العرض في مصمم التطبيق.</span><span class="sxs-lookup"><span data-stu-id="81028-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="81028-111">انتقل إلى مصمم التطبيق الخاص بالتطبيق المحدد ، واختر الكيان وطرق العرض الخاصة به ، وحدد طريقه العرض التي تريد تمكينها وحفظها ونشرها وإغلاقها.</span><span class="sxs-lookup"><span data-stu-id="81028-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="81028-112">تحديث الصفحة.</span><span class="sxs-lookup"><span data-stu-id="81028-112">Refresh the page.</span></span>