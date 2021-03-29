---
title: سير العمل لا يبدأ
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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403730"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="5dbd7-102">سير العمل لا يبدأ</span><span class="sxs-lookup"><span data-stu-id="5dbd7-102">Workflow is not starting</span></span>

- <span data-ttu-id="5dbd7-103">لم يبدأ سير عمل SharePoint 2010 و SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="5dbd7-104">إذا لم يبدأ سير العمل الخاص بك، فقد تكون هناك مشكلة خدمة مؤقتة حيث قد تواجه المستخدمين تأخيرات متقطعة مع تقدم سير العمل.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="5dbd7-105">تحقق من [لوحة معلومات حالة الخدمة](https://admin.microsoft.com/AdminPortal/Home/servicehealth) لمعرفة ما إذا كانت مؤسستك متأثّر بها.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="5dbd7-106">إذا مرت أكثر من 24 ساعة منذ أن رأيت هذه المشكلة للمرة الأولى، فالرجاء تسجيل تذكرة دعم.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="5dbd7-107">في العديد من الحالات، نحن نعمل بالفعل على إيجاد حل.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="5dbd7-108">الرجاء منحنا 24 ساعة على الأقل لإكمال الحل.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="5dbd7-109">تم تأخير مهام سير عمل SharePoint 2010 عند البدء.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="5dbd7-110">يحدث هذا الأمر إذا تم تشغيل سير العمل على دفعات كبيرة.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="5dbd7-111">(على سبيل المثال، عند إضافة عناصر متعددة في الوقت نفسه).</span><span class="sxs-lookup"><span data-stu-id="5dbd7-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="5dbd7-112">لم يتم تصميم مهام سير العمل بحيث تعمل في الوقت الحقيقي، لذا فإن التأخير هو سلوك التصميم حسب التصميم.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="5dbd7-113">إذا كان سير العمل عبارة عن لغة تمييز كائن (XMOL) معقدة، يمكن أن تكون عملية التحويل البرمجي بطيئة.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="5dbd7-114">تحقق [من هذه](https://support.microsoft.com//kb/3043697) المقالة.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="5dbd7-115">يجب تبسيط سير العمل أو إعادة تصميمه باستخدام نوع النظام الأساسي لسير عمل Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="5dbd7-116">إذا ازداد حجم محفوظات سير العمل، فقد ترغب في إزالة العناصر أو إنشاء قائمة محفوظات جديدة.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="5dbd7-117">مزيد من المعلومات : [إزالة محفوظات سير العمل](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="5dbd7-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="5dbd7-118">المواضيع ذات الصلة</span><span class="sxs-lookup"><span data-stu-id="5dbd7-118">Related topics</span></span>
<span data-ttu-id="5dbd7-119">هل تريد تجربة Microsoft Flow في SharePoint Online؟</span><span class="sxs-lookup"><span data-stu-id="5dbd7-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="5dbd7-120">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="5dbd7-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="5dbd7-121">SharePoint وتدفق</span><span class="sxs-lookup"><span data-stu-id="5dbd7-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
