---
title: القوائم الكبيرة في SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720120"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="30aa0-102">استخدام القوائم والمكتبات الكبيرة في SharePoint</span><span class="sxs-lookup"><span data-stu-id="30aa0-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="30aa0-103">يمكن ان تحتوي قوائم ومكتبات SharePoint علي ما يصل إلى 30,000,000 عنصر ، ولكن عندما يكون لديها أكثر من 5,000 عنصرا ، فقد تري خطا في عتبه طريقه عرض القائمة عند محاولة استخدامها.</span><span class="sxs-lookup"><span data-stu-id="30aa0-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="30aa0-104">يتواجد هذا الحد للحفاظ على أداء الخدمة.</span><span class="sxs-lookup"><span data-stu-id="30aa0-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="30aa0-105">ولا يمكن تغييره.</span><span class="sxs-lookup"><span data-stu-id="30aa0-105">It can't be changed.</span></span> <span data-ttu-id="30aa0-106">لتجنب الاصابه بهذا الحد:</span><span class="sxs-lookup"><span data-stu-id="30aa0-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="30aa0-107">**استخدام الحديثة**</span><span class="sxs-lookup"><span data-stu-id="30aa0-107">**Use modern**</span></span>

<span data-ttu-id="30aa0-108">تعمل طرق العرض التي تعرض العديد من العناصر بشكل أفضل في التجربة الحديثة.</span><span class="sxs-lookup"><span data-stu-id="30aa0-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="30aa0-109">[استخدم التجربة الحديثة](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) لتجنب الأخطاء التي قد تظهر في التجربة التقليدية.</span><span class="sxs-lookup"><span data-stu-id="30aa0-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="30aa0-110">**أضافه فهارس**</span><span class="sxs-lookup"><span data-stu-id="30aa0-110">**Add indexes**</span></span>

<span data-ttu-id="30aa0-111">عند اجراء تصفيه أو فرز حسب عمود لا يحتوي علي فهرس ، قد تظهر رسالة خطا.</span><span class="sxs-lookup"><span data-stu-id="30aa0-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="30aa0-112">[يمكنك أضافه فهرس](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) يدويا من " **إعدادات القائمة** " في القائمة "إعدادات" ، ثم **الاعمده المفهرسة**.</span><span class="sxs-lookup"><span data-stu-id="30aa0-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="30aa0-113">**تحرير طريقه عرض القائمة**</span><span class="sxs-lookup"><span data-stu-id="30aa0-113">**Edit the list view**</span></span>

<span data-ttu-id="30aa0-114">إذا ظهر خطا عند استخدام قائمه كبيره ، فقم [بتحرير طريقه عرض القائمة](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="30aa0-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="30aa0-115">ستؤدي التغييرات الاربعه التالية إلى أزاله الأخطاء الخاصة بطريقه عرض القائمة.</span><span class="sxs-lookup"><span data-stu-id="30aa0-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="30aa0-116">قم باجراء التغييرات الاربعه لأزاله كل الأخطاء.</span><span class="sxs-lookup"><span data-stu-id="30aa0-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="30aa0-117">إذا كنت لا تزال تواجه الأخطاء ، فراجع [أداره القوائم والمكتبات الكبيرة](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="30aa0-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="30aa0-118">حدد **بلا** من **الفرز الأول حسب العمود** ثم **قم بالفرز حسب العمود**.</span><span class="sxs-lookup"><span data-stu-id="30aa0-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="30aa0-119">حدد **بلا** من **المجموعة الاولي حسب العمود** ثم **قم بالتجميع حسب العمود**.</span><span class="sxs-lookup"><span data-stu-id="30aa0-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="30aa0-120">حدد **بلا** لكل الاعمده في المقطع **الإجماليات** .</span><span class="sxs-lookup"><span data-stu-id="30aa0-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="30aa0-121">إلغاء تحديد الكل ما عدا عمود واحد للعرض من مقطع **الاعمده** .</span><span class="sxs-lookup"><span data-stu-id="30aa0-121">Deselect all but one column for display from the **Columns** section.</span></span>

