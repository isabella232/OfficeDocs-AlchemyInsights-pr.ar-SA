---
title: تم تجاوز حد البريد الكتروني اليومي. تم تعليق سير العمل.
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
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053104"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="def43-103">تجاوز حد البريد الكتروني اليومي.</span><span class="sxs-lookup"><span data-stu-id="def43-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="def43-104">تم تعليق سير العمل.</span><span class="sxs-lookup"><span data-stu-id="def43-104">Workflow is suspended.</span></span>

<span data-ttu-id="def43-105">قد يتم تلقي هذا الخطا في السيناريوهات التالية:</span><span class="sxs-lookup"><span data-stu-id="def43-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="def43-106">لديك سير عمل في SharePoint علي الإنترنت التي تستخدم SharePoint 2010 أو SharePoint 2013 نوع النظام الأساسي سير العمل.</span><span class="sxs-lookup"><span data-stu-id="def43-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="def43-107">يتم تكوين سير العمل لإرسال رسالة بريد الكتروني مخصصه إلى أكثر من 200 المستخدمين في كل مره ، أكثر من 10,000 المستلمين في اليوم الواحد ، أو أكثر من 30 رسالة في الدقيقة الواحدة.</span><span class="sxs-lookup"><span data-stu-id="def43-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="def43-108">عند تشغيل سير العمل ، لا يتم إرسال رسالة البريد الكتروني ، ولاحظت السلوك التالي:</span><span class="sxs-lookup"><span data-stu-id="def43-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="def43-109">بالنسبة لسير العمل باستخدام نوع النظام الأساسي ل SharePoint 2013 ، يمكنك الاستعراض إلى صفحه **حاله سير العمل** .</span><span class="sxs-lookup"><span data-stu-id="def43-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="def43-110">في الصفحة "حاله سير العمل" ، يتم تعيين **الحالة الداخلية** إلى **البدء**، ويعرض بالون المعلومات **غير قادر علي إرسال إلى مستلم**.</span><span class="sxs-lookup"><span data-stu-id="def43-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="def43-111">كمحاولة للتغلب علي هذه المشكلة قم بتكوين سير العمل الخاص بك لإرسال رسائل البريد الكتروني دون تجاوز [حدود المرسل Exchange عبر إنترنت](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="def43-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="def43-112">علي سبيل المثال ، استخدم وقفه في سير العمل ، إرسال البريد الكتروني إلى مجموعه 365 Office أو مجموعه توزيع أو البريد تمكين مجموعه الأمان أو إرسال الرسالة إلى اقل من 200 المستلمين في كل مره.</span><span class="sxs-lookup"><span data-stu-id="def43-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="def43-113">لمزيد من المعلومات ، راجع [المقالة](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)التالية.</span><span class="sxs-lookup"><span data-stu-id="def43-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="def43-114">المواضيع ذات الصلة</span><span class="sxs-lookup"><span data-stu-id="def43-114">Related topics</span></span>
- [<span data-ttu-id="def43-115">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="def43-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="def43-116">SharePoint والتدفق</span><span class="sxs-lookup"><span data-stu-id="def43-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 