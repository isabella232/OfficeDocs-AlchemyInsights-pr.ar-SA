---
title: لا يتم الآن بدء تشغيل سير العمل
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
ms.openlocfilehash: efd17c302ae6d857207e87e94d74d3794e94a83a
ms.sourcegitcommit: 204be4a6ae03700b75eae6b09b4e9ab283089fbf
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/03/2019
ms.locfileid: "36171757"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="d228e-102">لا يتم الآن بدء تشغيل سير العمل</span><span class="sxs-lookup"><span data-stu-id="d228e-102">Workflow is not starting</span></span>

- <span data-ttu-id="d228e-103">مهام سير العمل SharePoint 2010 و SharePoint 2013 لا نبدأ.</span><span class="sxs-lookup"><span data-stu-id="d228e-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    <span data-ttu-id="d228e-104">إذا لم يبدأ سير العمل الخاص بك، قد يكون هناك مشكلة في خدمة مؤقت حيث المستخدمين قد تواجه تأخيرات متقطعة مع تقدم سير العمل.</span><span class="sxs-lookup"><span data-stu-id="d228e-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="d228e-105">تحقق من [لوحة المعلومات الصحية الخدمة](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) لترى إذا تأثر المؤسسة الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="d228e-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    <span data-ttu-id="d228e-106">لقد مرت أكثر من 24 ساعة منذ أول مرة في هذه المسألة، الرجاء تسجيل دعم تذكرة.</span><span class="sxs-lookup"><span data-stu-id="d228e-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="d228e-107">في كثير من الحالات، الفعل نعمل على إيجاد حل.</span><span class="sxs-lookup"><span data-stu-id="d228e-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="d228e-108">الرجاء إعطاء لنا أربع وعشرين ساعة لإكمال حل.</span><span class="sxs-lookup"><span data-stu-id="d228e-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="d228e-109">تأخير مهام سير العمل SharePoint 2010 عند بدء التشغيل.</span><span class="sxs-lookup"><span data-stu-id="d228e-109">SharePoint 2010 workflows delayed on start.</span></span>

    <span data-ttu-id="d228e-110">يحدث هذا إذا تم تشغيل سير العمل في مجموعات كبيرة.</span><span class="sxs-lookup"><span data-stu-id="d228e-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="d228e-111">(على سبيل المثال، عند عدة عناصر تضاف مرة واحدة).</span><span class="sxs-lookup"><span data-stu-id="d228e-111">(for example, when several items are added at once).</span></span>

    <span data-ttu-id="d228e-112">مهام سير العمل غير مصممة لتعمل في الوقت الحقيقي، وبالتالي تأخير هو السلوك حسب التصميم.</span><span class="sxs-lookup"><span data-stu-id="d228e-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

    <span data-ttu-id="d228e-113">إذا كان سير العمل تعقيداً الموسعة كائن ترميز اللغة (إكسمول)، يمكن أن يكون التحويل البرمجي بطيئا.</span><span class="sxs-lookup"><span data-stu-id="d228e-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="d228e-114">التحقق من [هذه](https://support.microsoft.com/en-us/kb/3043697) المادة.</span><span class="sxs-lookup"><span data-stu-id="d228e-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    <span data-ttu-id="d228e-115">وينبغي تبسيط سير العمل أو إعادة تصميم استخدام نوع النظام الأساسي ل Microsoft SharePoint 2013 سير العمل.</span><span class="sxs-lookup"><span data-stu-id="d228e-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    <span data-ttu-id="d228e-116">أيضا، إذا أصبحت كبيرة محفوظات سير العمل الخاصة بك، قد تحتاج إلى حذف العناصر أو قم بإنشاء قائمة محفوظات.</span><span class="sxs-lookup"><span data-stu-id="d228e-116">Also, if your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

    <span data-ttu-id="d228e-117">مزيد من المعلومات: [مسح محفوظات سير العمل](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="d228e-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="d228e-118">المواضيع ذات الصلة</span><span class="sxs-lookup"><span data-stu-id="d228e-118">Related topics</span></span>
<span data-ttu-id="d228e-119">هل ترغب في محاولة تدفق Micrsoft في SharePoint عبر إنترنت؟</span><span class="sxs-lookup"><span data-stu-id="d228e-119">Want to try Micrsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="d228e-120">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="d228e-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="d228e-121">SharePoint والتدفق</span><span class="sxs-lookup"><span data-stu-id="d228e-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


