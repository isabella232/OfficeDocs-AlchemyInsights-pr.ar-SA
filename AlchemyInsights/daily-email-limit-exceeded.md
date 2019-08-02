---
title: تم تجاوز حد البريد الإلكتروني يوميا. يتم تعطيل سير العمل.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059626"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="dfdd1-103">تجاوز حد البريد الإلكتروني يوميا.</span><span class="sxs-lookup"><span data-stu-id="dfdd1-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="dfdd1-104">يتم تعطيل سير العمل.</span><span class="sxs-lookup"><span data-stu-id="dfdd1-104">Workflow is suspended.</span></span>

<span data-ttu-id="dfdd1-105">وقد تلقي هذا الخطأ في السيناريوهات التالية:</span><span class="sxs-lookup"><span data-stu-id="dfdd1-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="dfdd1-106">يكون سير عمل في SharePoint على الإنترنت الذي يستخدم SharePoint 2010 أو نوع النظام الأساسي لسير العمل SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="dfdd1-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="dfdd1-107">تم تكوين سير العمل لإرسال رسالة بريد إلكتروني مخصصة للمستخدمين أكثر من 200 في مرة الواحدة أو المستلمين أكثر من 10 آلاف يوميا أكثر من 30 رسالة في الدقيقة.</span><span class="sxs-lookup"><span data-stu-id="dfdd1-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="dfdd1-108">عندما تقوم بتشغيل سير العمل، لم يتم إرسال رسالة البريد الإلكتروني، ولاحظت السلوك التالي:</span><span class="sxs-lookup"><span data-stu-id="dfdd1-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="dfdd1-109">لسير عمل باستخدام نوع النظام الأساسي SharePoint 2013، يمكنك استعراض الصفحة " **حالة سير العمل** ".</span><span class="sxs-lookup"><span data-stu-id="dfdd1-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="dfdd1-110">في الصفحة "حالة سير العمل"، يتم تعيين **الحالة الداخلية** **الشروع في العمل**، ويعرض بالون معلومات **قادر على إرسال إلى مستلم**.</span><span class="sxs-lookup"><span data-stu-id="dfdd1-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="dfdd1-111">للتغلب على هذه المشكلة، قم بتكوين سير العمل الخاص بك لإرسال رسائل البريد الإلكتروني دون تجاوز [حدود المرسل Exchange عبر إنترنت](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="dfdd1-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="dfdd1-112">على سبيل المثال، استخدم مؤقتاً في سير العمل إرسال البريد الإلكتروني إلى مجموعة Office 365، مجموعة توزيع أو مجموعة أمان تمكين البريد أو إرسال الرسالة إلى المستلمين أقل من 200 في نفس وقت.</span><span class="sxs-lookup"><span data-stu-id="dfdd1-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="dfdd1-113">لمزيد من المعلومات، راجع [المقالة](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)التالية.</span><span class="sxs-lookup"><span data-stu-id="dfdd1-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="dfdd1-114">المواضيع ذات الصلة</span><span class="sxs-lookup"><span data-stu-id="dfdd1-114">Related topics</span></span>
- [<span data-ttu-id="dfdd1-115">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="dfdd1-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="dfdd1-116">SharePoint والتدفق</span><span class="sxs-lookup"><span data-stu-id="dfdd1-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 