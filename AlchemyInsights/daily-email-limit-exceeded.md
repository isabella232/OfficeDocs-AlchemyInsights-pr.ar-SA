---
title: تم تجاوز حد البريد الكتروني اليومي. تم إيقاف سير العمل.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731550"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="04a48-103">تم تجاوز حد البريد الكتروني اليومي.</span><span class="sxs-lookup"><span data-stu-id="04a48-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="04a48-104">تم إيقاف سير العمل.</span><span class="sxs-lookup"><span data-stu-id="04a48-104">Workflow is suspended.</span></span>

<span data-ttu-id="04a48-105">قد يتم استلام هذا الخطا في السيناريوهات التالية:</span><span class="sxs-lookup"><span data-stu-id="04a48-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="04a48-106">لديك سير عمل في SharePoint Online يستخدم نوع النظام الأساسي لسير العمل SharePoint 2010 أو SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="04a48-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="04a48-107">تم تكوين سير العمل لإرسال رسالة بريد الكتروني مخصصه إلى أكثر من 200 مستخدمين في نفس الوقت ، أو أكثر من 10,000 مستلم في اليوم ، أو أكثر من 30 رسالة في الدقيقة.</span><span class="sxs-lookup"><span data-stu-id="04a48-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="04a48-108">عند تشغيل سير العمل ، لا يتم إرسال رسالة البريد الكتروني ، وتلاحظ السلوك التالي:</span><span class="sxs-lookup"><span data-stu-id="04a48-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="04a48-109">بالنسبة لسير العمل باستخدام نوع النظام الأساسي ل SharePoint 2013 ، يمكنك الاستعراض وصولا إلى الصفحة " **حاله سير العمل** ".</span><span class="sxs-lookup"><span data-stu-id="04a48-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="04a48-110">في الصفحة "حاله سير العمل" ، يتم تعيين **الحالة الداخلية** إلى " **تم البدء**" ، ويتم عرض بالون المعلومات **غير قادر علي الإرسال إلى المستلم**.</span><span class="sxs-lookup"><span data-stu-id="04a48-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="04a48-111">لحل هذه المشكلة ، قم بتكوين سير العمل لإرسال رسائل البريد الكتروني بدون تجاوز [حدود مرسل Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="04a48-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="04a48-112">علي سبيل المثال ، يمكنك استخدام إيقاف مؤقت في سير العمل ، أو إرسال البريد الكتروني إلى مجموعه Microsoft 365 ، أو مجموعه توزيع أو مجموعه أمان ممكنة ، أو إرسال الرسالة إلى اقل من 200 مستلم في الوقت نفسه.</span><span class="sxs-lookup"><span data-stu-id="04a48-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="04a48-113">لمزيد من المعلومات ، راجع [المقالة](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)التالية.</span><span class="sxs-lookup"><span data-stu-id="04a48-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="04a48-114">المواضيع ذات الصلة</span><span class="sxs-lookup"><span data-stu-id="04a48-114">Related topics</span></span>
- [<span data-ttu-id="04a48-115">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="04a48-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="04a48-116">SharePoint والتدفق</span><span class="sxs-lookup"><span data-stu-id="04a48-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 