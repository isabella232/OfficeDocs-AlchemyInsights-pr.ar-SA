---
title: لم يبدأ سير العمل
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766084"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="28156-102">لم يبدأ سير العمل</span><span class="sxs-lookup"><span data-stu-id="28156-102">Workflow is not starting</span></span>

- <span data-ttu-id="28156-103">لم يتم بدء سير عمل SharePoint 2010 و SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="28156-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="28156-104">إذا لم يبدأ سير العمل، فقد تكون هناك مشكلة خدمة مؤقتة حيث قد يواجه المستخدمون تأخيرات متقطعة مع تقدم سير العمل.</span><span class="sxs-lookup"><span data-stu-id="28156-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="28156-105">تحقق من [لوحة معلومات صحة الخدمة](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) لمعرفة ما إذا كانت مؤسستك متأثرة.</span><span class="sxs-lookup"><span data-stu-id="28156-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="28156-106">إذا مرت أكثر من 24 ساعة منذ أن رأيت هذه المشكلة لأول مرة، يرجى تسجيل تذكرة دعم.</span><span class="sxs-lookup"><span data-stu-id="28156-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="28156-107">في كثير من الحالات، نحن نعمل بالفعل على حل.</span><span class="sxs-lookup"><span data-stu-id="28156-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="28156-108">يرجى من خلالنا أن تعطينا 24 ساعة على الأقل لإكمال الحل.</span><span class="sxs-lookup"><span data-stu-id="28156-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="28156-109">تأخر سير عمل SharePoint 2010 في البداية.</span><span class="sxs-lookup"><span data-stu-id="28156-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="28156-110">يحدث هذا إذا تم تشغيل سير العمل على دفعات كبيرة.</span><span class="sxs-lookup"><span data-stu-id="28156-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="28156-111">(على سبيل المثال، عند إضافة عدة عناصر في وقت واحد).</span><span class="sxs-lookup"><span data-stu-id="28156-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="28156-112">لم يتم تصميم مهام سير العمل لتشغيلها في الوقت الفعلي، لذلك فإن التأخير هو سلوك حسب التصميم.</span><span class="sxs-lookup"><span data-stu-id="28156-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="28156-113">إذا كان سير العمل هو لغة ترميز كائن قابلة للتوسعة المعقدة (XMOL)، يمكن أن يكون التحويل البرمجي بطيئاً.</span><span class="sxs-lookup"><span data-stu-id="28156-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="28156-114">تحقق من [هذه](https://support.microsoft.com//kb/3043697) المقالة.</span><span class="sxs-lookup"><span data-stu-id="28156-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="28156-115">يجب تبسيط سير العمل أو إعادة تصميمه باستخدام نوع نظام Microsoft SharePoint 2013 الأساسي لسير العمل.</span><span class="sxs-lookup"><span data-stu-id="28156-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="28156-116">إذا كان سجل سير العمل الخاص بك قد نما بشكل كبير، فقد تحتاج إلى تطهير العناصر أو إنشاء قائمة محفوظات جديدة.</span><span class="sxs-lookup"><span data-stu-id="28156-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="28156-117">مزيد من المعلومات : [تطهير محفوظات سير العمل](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="28156-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="28156-118">المواضيع ذات الصلة</span><span class="sxs-lookup"><span data-stu-id="28156-118">Related topics</span></span>
<span data-ttu-id="28156-119">هل تريد تجربة Microsoft Flow في SharePoint Online؟</span><span class="sxs-lookup"><span data-stu-id="28156-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="28156-120">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="28156-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="28156-121">SharePoint والتدفق</span><span class="sxs-lookup"><span data-stu-id="28156-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


