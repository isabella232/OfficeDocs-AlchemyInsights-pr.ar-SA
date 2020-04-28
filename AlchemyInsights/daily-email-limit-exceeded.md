---
title: تجاوز حد البريد الإلكتروني اليومي. تم تعليق سير العمل.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 5a510f1137c7c49cd1de3d3fd2a470759e37ba1e
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908691"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="41d2e-103">تجاوز حد البريد الإلكتروني اليومي.</span><span class="sxs-lookup"><span data-stu-id="41d2e-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="41d2e-104">تم تعليق سير العمل.</span><span class="sxs-lookup"><span data-stu-id="41d2e-104">Workflow is suspended.</span></span>

<span data-ttu-id="41d2e-105">قد يتم تلقي هذا الخطأ في السيناريوهات التالية:</span><span class="sxs-lookup"><span data-stu-id="41d2e-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="41d2e-106">لديك سير عمل في SharePoint Online يستخدم نوع منصة سير عمل SharePoint 2010 أو SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="41d2e-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="41d2e-107">تم تكوين سير العمل لإرسال رسالة بريد إلكتروني مخصصة إلى أكثر من 200 مستخدم في وقت واحد، أو أكثر من 10,000 مستلم يوميًا، أو أكثر من 30 رسالة في الدقيقة.</span><span class="sxs-lookup"><span data-stu-id="41d2e-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="41d2e-108">عند تشغيل سير العمل، لا يتم إرسال رسالة البريد الإلكتروني، وتلاحظ السلوك التالي:</span><span class="sxs-lookup"><span data-stu-id="41d2e-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="41d2e-109">بالنسبة لسير العمل باستخدام نوع النظام الأساسي SharePoint 2013، يمكنك الاستعراض إلى صفحة **حالة سير العمل.**</span><span class="sxs-lookup"><span data-stu-id="41d2e-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="41d2e-110">في صفحة حالة سير العمل، يتم تعيين **الحالة الداخلية** إلى **"تم البدء"،** ويعرض بالون المعلومات **غير قادر على الإرسال إلى مستلم**.</span><span class="sxs-lookup"><span data-stu-id="41d2e-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="41d2e-111">لحل هذه المشكلة، قم بتكوين سير العمل لإرسال رسائل البريد الإلكتروني دون تجاوز [حدود المرسل Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="41d2e-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="41d2e-112">على سبيل المثال، استخدم إيقافمؤقت في سير العمل، أو إرسال البريد الإلكتروني إلى مجموعة Microsoft 365 أو مجموعة توزيع أو مجموعة أمان ممكّنة للبريد، أو إرسال الرسالة إلى أقل من 200 مستلم في كل مرة.</span><span class="sxs-lookup"><span data-stu-id="41d2e-112">For example, use a pause in the workflow, send the email to an Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="41d2e-113">لمزيد من المعلومات، راجع [المقالة](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)التالية .</span><span class="sxs-lookup"><span data-stu-id="41d2e-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="41d2e-114">المواضيع ذات الصلة</span><span class="sxs-lookup"><span data-stu-id="41d2e-114">Related topics</span></span>
- [<span data-ttu-id="41d2e-115">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="41d2e-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="41d2e-116">SharePoint والتدفق</span><span class="sxs-lookup"><span data-stu-id="41d2e-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 