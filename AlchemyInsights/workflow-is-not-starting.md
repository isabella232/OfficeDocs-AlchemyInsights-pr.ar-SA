---
title: لم يتم بدء تشغيل سير العمل
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36738076"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="237ac-102">لم يتم بدء تشغيل سير العمل</span><span class="sxs-lookup"><span data-stu-id="237ac-102">Workflow is not starting</span></span>

- <span data-ttu-id="237ac-103">لم يتم بدء تشغيل مهام سير العمل SharePoint 2010 و SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="237ac-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="237ac-104">إذا لم يتم بدء سير العمل ، قد تكون هناك مشكله خدمه مؤقته حيث قد يواجه المستخدمون تاخيرات متقطعه مع تقدم سير العمل.</span><span class="sxs-lookup"><span data-stu-id="237ac-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="237ac-105">تحقق من [لوحه معلومات صحة الخدمة](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) لمعرفه ما إذا كانت مؤسستك قد تاثرت.</span><span class="sxs-lookup"><span data-stu-id="237ac-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="237ac-106">إذا مرت أكثر من 24 ساعة منذ ان رايت هذه المسالة لأول مره ، يرجى تسجيل تذكره الدعم.</span><span class="sxs-lookup"><span data-stu-id="237ac-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="237ac-107">في كثير من الحالات ، نحن نعمل بالفعل علي حل.</span><span class="sxs-lookup"><span data-stu-id="237ac-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="237ac-108">من فضلك أعطنا 24 ساعة علي الأقل لإكمال الحل.</span><span class="sxs-lookup"><span data-stu-id="237ac-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="237ac-109">تاخير مهام سير العمل 2010 SharePoint علي البدء.</span><span class="sxs-lookup"><span data-stu-id="237ac-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="237ac-110">يحدث هذا إذا تم تشغيل سير العمل في دفعات كبيره.</span><span class="sxs-lookup"><span data-stu-id="237ac-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="237ac-111">(علي سبيل المثال ، عند أضافه العديد من العناصر في وقت واحد).</span><span class="sxs-lookup"><span data-stu-id="237ac-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="237ac-112">لم يتم تصميم مهام سير العمل ليتم تشغيلها في الوقت الحقيقي ، التالي فان التاخير هو سلوك تصميمي.</span><span class="sxs-lookup"><span data-stu-id="237ac-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="237ac-113">إذا كان سير العمل عبارة عن لغة توصيف الكائنات القابلة للتوسيع (XMOL) معقده ، يمكن ان يكون التحويل البرمجي بطيئا.</span><span class="sxs-lookup"><span data-stu-id="237ac-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="237ac-114">تحقق من [هذه](https://support.microsoft.com//kb/3043697) المقالة.</span><span class="sxs-lookup"><span data-stu-id="237ac-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="237ac-115">يجب تبسيط سير العمل أو أعاده تصميمه باستخدام نوع النظام الأساسي ل Microsoft SharePoint 2013 سير العمل.</span><span class="sxs-lookup"><span data-stu-id="237ac-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="237ac-116">إذا نما سجل سير العمل الخاص بك كبير ، قد تحتاج إلى أزاله العناصر أو إنشاء قائمه محفوظات جديده.</span><span class="sxs-lookup"><span data-stu-id="237ac-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="237ac-117">مزيد من المعلومات: [أزاله محفوظات سير العمل](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="237ac-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="237ac-118">المواضيع ذات الصلة</span><span class="sxs-lookup"><span data-stu-id="237ac-118">Related topics</span></span>
<span data-ttu-id="237ac-119">هل تريد محاولة Microsoft Flow في SharePoint علي الإنترنت ؟</span><span class="sxs-lookup"><span data-stu-id="237ac-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="237ac-120">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="237ac-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="237ac-121">SharePoint والتدفق</span><span class="sxs-lookup"><span data-stu-id="237ac-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


