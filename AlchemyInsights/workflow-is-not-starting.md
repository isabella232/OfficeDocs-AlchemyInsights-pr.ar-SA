---
title: لا يتم بدء سير العمل
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794754"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="89cd7-102">لا يتم بدء سير العمل</span><span class="sxs-lookup"><span data-stu-id="89cd7-102">Workflow is not starting</span></span>

- <span data-ttu-id="89cd7-103">لا يتم بدء تشغيل مهام سير عمل SharePoint 2010 و SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="89cd7-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="89cd7-104">إذا لم يتم بدء تشغيل سير العمل الخاص بك ، فقد يكون هناك مشكله خدمه مؤقته حيث يواجه المستخدمون تاخيرات متقطعه مع تقدم سير العمل.</span><span class="sxs-lookup"><span data-stu-id="89cd7-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="89cd7-105">راجع [لوحه معلومات حماية الخدمة](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) لمعرفه ما إذا كانت مؤسستك متاثره بالأمر.</span><span class="sxs-lookup"><span data-stu-id="89cd7-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="89cd7-106">إذا تم تمرير أكثر من 24 ساعة منذ المرة الاولي التي قمت فيها بمشاهده هذه المشكلة ، يرجى تسجيل تذكره دعم.</span><span class="sxs-lookup"><span data-stu-id="89cd7-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="89cd7-107">في حالات كثيره ، نحن نعمل بالفعل علي حل.</span><span class="sxs-lookup"><span data-stu-id="89cd7-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="89cd7-108">يرجى تقديم 24 ساعة علي الأقل لإكمال حل.</span><span class="sxs-lookup"><span data-stu-id="89cd7-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="89cd7-109">تم تاخير مهام سير عمل SharePoint 2010 في البداية.</span><span class="sxs-lookup"><span data-stu-id="89cd7-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="89cd7-110">يحدث هذا إذا تم تشغيل سير العمل في دفعات كبيره.</span><span class="sxs-lookup"><span data-stu-id="89cd7-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="89cd7-111">(علي سبيل المثال ، عند أضافه عناصر متعددة في وقت واحد).</span><span class="sxs-lookup"><span data-stu-id="89cd7-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="89cd7-112">لا يتم تصميم مهام سير العمل ليتم تشغيلها في الوقت الحقيقي ، التالي فان التاخير هو السلوك بالتصميم.</span><span class="sxs-lookup"><span data-stu-id="89cd7-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="89cd7-113">إذا كان سير العمل عبارة عن لغة تمييز معقده للعناصر (إكسمول) ، فقد يكون التحويل البرمجي بطيئا.</span><span class="sxs-lookup"><span data-stu-id="89cd7-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="89cd7-114">راجع [هذه](https://support.microsoft.com//kb/3043697) المقالة.</span><span class="sxs-lookup"><span data-stu-id="89cd7-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="89cd7-115">ينبغي عليك تبسيط سير العمل أو أعاده تصميمه باستخدام نوع النظام الأساسي لسير العمل Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="89cd7-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="89cd7-116">إذا كانت محفوظات سير العمل كبيره جدا ، فقد ترغب في أزاله العناصر أو إنشاء قائمه محفوظات جديده.</span><span class="sxs-lookup"><span data-stu-id="89cd7-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="89cd7-117">مزيد من المعلومات: [أزاله محفوظات سير العمل](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="89cd7-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="89cd7-118">المواضيع ذات الصلة</span><span class="sxs-lookup"><span data-stu-id="89cd7-118">Related topics</span></span>
<span data-ttu-id="89cd7-119">هل تريد تجربه Microsoft تدفق في SharePoint Online ؟</span><span class="sxs-lookup"><span data-stu-id="89cd7-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="89cd7-120">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="89cd7-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="89cd7-121">SharePoint والتدفق</span><span class="sxs-lookup"><span data-stu-id="89cd7-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


