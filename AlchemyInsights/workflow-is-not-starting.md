---
title: لم يبدأ سير العمل
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
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36738076"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="8df2c-102">لم يبدأ سير العمل</span><span class="sxs-lookup"><span data-stu-id="8df2c-102">Workflow is not starting</span></span>

- <span data-ttu-id="8df2c-103">لم يتم بدء تشغيل مهام سير عمل SharePoint 2010 و SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="8df2c-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="8df2c-104">إذا لم يتم بدء تشغيل سير العمل الخاص بك، قد تكون هناك مشكلة خدمة مؤقتة حيث قد يواجه المستخدمون تأخيرات متقطعة مع تقدم سير العمل.</span><span class="sxs-lookup"><span data-stu-id="8df2c-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="8df2c-105">تحقق من [لوحة معلومات صحة الخدمة](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) لمعرفة ما إذا كانت مؤسستك قد تأثرت.</span><span class="sxs-lookup"><span data-stu-id="8df2c-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="8df2c-106">إذا مرت أكثر من 24 ساعة منذ أن رأيت هذه المشكلة لأول مرة، الرجاء تسجيل تذكرة دعم.</span><span class="sxs-lookup"><span data-stu-id="8df2c-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="8df2c-107">في كثير من الحالات، نحن نعمل بالفعل على حل.</span><span class="sxs-lookup"><span data-stu-id="8df2c-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="8df2c-108">يرجى تعطينا ما لا يقل عن 24 ساعة لاستكمال حل.</span><span class="sxs-lookup"><span data-stu-id="8df2c-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="8df2c-109">تأخر مهام سير عمل SharePoint 2010 عند البدء.</span><span class="sxs-lookup"><span data-stu-id="8df2c-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="8df2c-110">يحدث هذا إذا تم تشغيل سير العمل في دفعات كبيرة.</span><span class="sxs-lookup"><span data-stu-id="8df2c-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="8df2c-111">(على سبيل المثال، عند إضافة العديد من العناصر في وقت واحد).</span><span class="sxs-lookup"><span data-stu-id="8df2c-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="8df2c-112">لم يتم تصميم مهام سير العمل لتشغيل في الوقت الحقيقي، لذلك التأخير هو سلوك التصميم حسب التصميم.</span><span class="sxs-lookup"><span data-stu-id="8df2c-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="8df2c-113">إذا كان سير العمل معقد لغة توصيف الكائنات الموسعة (XMOL)، يمكن أن يكون التحويل البرمجي بطيئاً.</span><span class="sxs-lookup"><span data-stu-id="8df2c-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="8df2c-114">تحقق من [هذه](https://support.microsoft.com//kb/3043697) المقالة.</span><span class="sxs-lookup"><span data-stu-id="8df2c-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="8df2c-115">يجب تبسيط سير العمل أو إعادة تصميمه باستخدام نوع النظام الأساسي لسير عمل Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="8df2c-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="8df2c-116">إذا كان سجل سير العمل قد نما كبيرًا، فقد تحتاج إلى إزالة العناصر أو إنشاء قائمة محفوظات جديدة.</span><span class="sxs-lookup"><span data-stu-id="8df2c-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="8df2c-117">مزيد من المعلومات : [إزالة محفوظات سير العمل](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="8df2c-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="8df2c-118">المواضيع ذات الصلة</span><span class="sxs-lookup"><span data-stu-id="8df2c-118">Related topics</span></span>
<span data-ttu-id="8df2c-119">هل تريد تجربة تدفق Microsoft في SharePoint عبر الإنترنت؟</span><span class="sxs-lookup"><span data-stu-id="8df2c-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="8df2c-120">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="8df2c-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="8df2c-121">SharePoint والتدفق</span><span class="sxs-lookup"><span data-stu-id="8df2c-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


