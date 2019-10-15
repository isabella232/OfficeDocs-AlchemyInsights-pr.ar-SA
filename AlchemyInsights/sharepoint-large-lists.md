---
title: قوائم SharePoint الكبيرة
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488504"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="a67d1-102">العمل مع القوائم والمكتبات الكبيرة في SharePoint</span><span class="sxs-lookup"><span data-stu-id="a67d1-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="a67d1-103">يمكن ان تحتوي قوائم ومكتبات SharePoint علي ما يصل إلى 30,000,000 عنصرا ، ولكن عندما يكون لديهم أكثر من 5,000 عنصرا ، فقد يظهر لك خطا "عتبه طريقه عرض القائمة" عند محاولة العمل معهم.</span><span class="sxs-lookup"><span data-stu-id="a67d1-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="a67d1-104">وهذه العتبة قائمه للمحافظة علي أداء الخدمة.</span><span class="sxs-lookup"><span data-stu-id="a67d1-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="a67d1-105">لا يمكن تغييره</span><span class="sxs-lookup"><span data-stu-id="a67d1-105">It can't be changed.</span></span> <span data-ttu-id="a67d1-106">لتجنب ضرب هذه العتبة:</span><span class="sxs-lookup"><span data-stu-id="a67d1-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="a67d1-107">**استخدام الحديث**</span><span class="sxs-lookup"><span data-stu-id="a67d1-107">**Use modern**</span></span>

<span data-ttu-id="a67d1-108">المشاهدات التي تظهر العديد من العناصر تعمل بشكل أفضل في التجربة الحديثة.</span><span class="sxs-lookup"><span data-stu-id="a67d1-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="a67d1-109">[استخدم التجربة الحديثة](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) لتجنب الأخطاء التي قد تراها في التجربة الكلاسيكية.</span><span class="sxs-lookup"><span data-stu-id="a67d1-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="a67d1-110">**أضافه فهارس**</span><span class="sxs-lookup"><span data-stu-id="a67d1-110">**Add indexes**</span></span>

<span data-ttu-id="a67d1-111">عندما تقوم بالتصفية أو الفرز حسب عمود لا يوجد به فهرس ، قد تظهر لك رسالة خطا.</span><span class="sxs-lookup"><span data-stu-id="a67d1-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="a67d1-112">[أضافه فهرس](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) يدويا من **قائمه إعدادات** في قائمه الإعدادات ، ثم **الاعمده المفهرسة**.</span><span class="sxs-lookup"><span data-stu-id="a67d1-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="a67d1-113">**تحرير طريقه عرض القائمة**</span><span class="sxs-lookup"><span data-stu-id="a67d1-113">**Edit the list view**</span></span>

<span data-ttu-id="a67d1-114">في حاله حدوث خطا عند العمل مع قائمه كبيره ، قم [بتحرير طريقه عرض القائمة](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="a67d1-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="a67d1-115">ستقوم التغييرات الاربعه التالية بازاله أخطاء عتبه عرض القائمة.</span><span class="sxs-lookup"><span data-stu-id="a67d1-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="a67d1-116">اجراء كافة التغييرات الاربعه لأزاله كافة الأخطاء.</span><span class="sxs-lookup"><span data-stu-id="a67d1-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="a67d1-117">إذا كنت لا تزال تحصل علي أخطاء ، فتحقق من [أداره القوائم والمكتبات الكبيرة](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="a67d1-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="a67d1-118">حدد **لا شيء** من كل من **الفرز الأول حسب العمود** **ثم قم بالفرز حسب العمود**.</span><span class="sxs-lookup"><span data-stu-id="a67d1-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="a67d1-119">حدد **بلا** من **المجموعة الاولي بواسطة العمود** **ثم قم بتجميع حسب العمود**.</span><span class="sxs-lookup"><span data-stu-id="a67d1-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="a67d1-120">حدد **بلا** لكافة الاعمده في قسم **المجاميع** .</span><span class="sxs-lookup"><span data-stu-id="a67d1-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="a67d1-121">قم بإلغاء تحديد كل عمود ولكن للعرض من قسم **الاعمده** .</span><span class="sxs-lookup"><span data-stu-id="a67d1-121">Deselect all but one column for display from the **Columns** section.</span></span>

