---
title: قوائم SharePoint الكبيرة
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767272"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="4beb9-102">العمل مع القوائم الكبيرة والمكتبات في SharePoint</span><span class="sxs-lookup"><span data-stu-id="4beb9-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="4beb9-103">يمكن أن تحتوي قوائم SharePoint والمكتبات على ما يصل إلى 30 مليون عنصر، ولكن عندما تحتوي على أكثر من 5000 عنصر، قد ترى خطأ عتبة عرض القائمة عند محاولة العمل معها.</span><span class="sxs-lookup"><span data-stu-id="4beb9-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="4beb9-104">يتواجد هذا الحد للحفاظ على أداء الخدمة.</span><span class="sxs-lookup"><span data-stu-id="4beb9-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="4beb9-105">ولا يمكن تغييره.</span><span class="sxs-lookup"><span data-stu-id="4beb9-105">It can't be changed.</span></span> <span data-ttu-id="4beb9-106">لتجنب ضرب هذه العتبة:</span><span class="sxs-lookup"><span data-stu-id="4beb9-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="4beb9-107">**استخدام الحديثة**</span><span class="sxs-lookup"><span data-stu-id="4beb9-107">**Use modern**</span></span>

<span data-ttu-id="4beb9-108">وجهات النظر التي تبين العديد من العناصر تعمل بشكل أفضل في التجربة الحديثة.</span><span class="sxs-lookup"><span data-stu-id="4beb9-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="4beb9-109">[استخدم التجربة الحديثة](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) لتجنب الأخطاء التي قد تراها في التجربة الكلاسيكية.</span><span class="sxs-lookup"><span data-stu-id="4beb9-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="4beb9-110">**إضافة فهارس**</span><span class="sxs-lookup"><span data-stu-id="4beb9-110">**Add indexes**</span></span>

<span data-ttu-id="4beb9-111">عند التصفية أو الفرز حسب عمود لا يحتوي على فهرس، قد ترى رسالة خطأ.</span><span class="sxs-lookup"><span data-stu-id="4beb9-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="4beb9-112">[إضافة فهرس](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) يدوياً من **إعدادات القائمة** في قائمة الإعدادات، ثم **الأعمدة المفهرسة**.</span><span class="sxs-lookup"><span data-stu-id="4beb9-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="4beb9-113">**تحرير طريقة عرض القائمة**</span><span class="sxs-lookup"><span data-stu-id="4beb9-113">**Edit the list view**</span></span>

<span data-ttu-id="4beb9-114">في حالة حدوث خطأ عند العمل مع قائمة كبيرة، [قم بتحرير طريقة عرض القائمة](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="4beb9-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="4beb9-115">ستزيل التغييرات الأربعة التالية أخطاء عتبة عرض القائمة.</span><span class="sxs-lookup"><span data-stu-id="4beb9-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="4beb9-116">إجراء كافة التغييرات الأربعة لإزالة كافة الأخطاء.</span><span class="sxs-lookup"><span data-stu-id="4beb9-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="4beb9-117">إذا كنت لا تزال تحصل على أخطاء، تحقق [من إدارة القوائم الكبيرة والمكتبات](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="4beb9-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="4beb9-118">**حدد بلا** من الفرز الأول **حسب العمود** ثم **قم بالفرز حسب العمود**.</span><span class="sxs-lookup"><span data-stu-id="4beb9-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="4beb9-119">**حدد بلا** من كل من المجموعة الأولى **حسب العمود** ثم **قم بالتجميع حسب العمود**.</span><span class="sxs-lookup"><span data-stu-id="4beb9-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="4beb9-120">**حدد بلا** لكافة الأعمدة في قسم **الإجماليات.**</span><span class="sxs-lookup"><span data-stu-id="4beb9-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="4beb9-121">إلغاء تحديد كافة الأعمدة باستثناء عمود واحد للعرض من قسم **الأعمدة.**</span><span class="sxs-lookup"><span data-stu-id="4beb9-121">Deselect all but one column for display from the **Columns** section.</span></span>

