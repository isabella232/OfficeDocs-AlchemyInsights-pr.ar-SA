---
title: التعليقات في Microsoft Planner
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001717"
- "3810"
ms.openlocfilehash: 09385fd0235939d01e0baf141362cb8b76910682
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817627"
---
# <a name="comments-in-microsoft-planner"></a><span data-ttu-id="a663c-102">التعليقات في Microsoft Planner</span><span class="sxs-lookup"><span data-stu-id="a663c-102">Comments in Microsoft Planner</span></span>

<span data-ttu-id="a663c-103">يتم تخزين تعليقات المهام الموجودة في خطة في علبة بريد Exchange Online لمجموعة Microsoft 365 المقترنة بالخطة.</span><span class="sxs-lookup"><span data-stu-id="a663c-103">Comments for tasks within a plan are stored in the Exchange Online mailbox for the Microsoft 365 Group associated with the plan.</span></span>  <span data-ttu-id="a663c-104">عند نشر تعليق علي مهمة ما، يتم إرسال إعلام بالبريد الإلكتروني إلى علبة الوارد الخاصة بالمجموعة، ثم ستتلقى رسالة بريد إلكتروني لكل تعليق تال تم إجراؤه علي هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="a663c-104">When you post a comment on a task, an email notification is sent to the group inbox, and you will receive an email for each subsequent comment made on that task.</span></span>

<span data-ttu-id="a663c-105">فيما يلي بعض الإجابات حول المشاكل الشائعة المتعلقة بالتعليقات:</span><span class="sxs-lookup"><span data-stu-id="a663c-105">Here are some answers to common issues related to comments:</span></span>

- <span data-ttu-id="a663c-106">**لا يتلقى المستخدمون رسائل البريد الإلكتروني** - تيتم إرسال التعليقات إلى صندوق بريد المجموعة الخاص بالمجموعة التي تنتمي إليها الخطة.</span><span class="sxs-lookup"><span data-stu-id="a663c-106">**Users are not receiving emails** - Comments are sent to the group inbox for the group the plan belongs to.</span></span> <span data-ttu-id="a663c-107">لكي يتلقى المستخدم رسائل البريد الإلكتروني للمجموعة، يجب تكوين المجموعة لإرسال محادثات المجموعة إلى البريد الوارد للعضو.</span><span class="sxs-lookup"><span data-stu-id="a663c-107">For a user to receive group emails, the group should be configured to send group conversations to member's inboxes.</span></span>

- <span data-ttu-id="a663c-108">**لا يتم حفظ التعليقات** -  ليس لدى المستخدم الذي يضيف التعليق الإذن لإرسال بريد إلكتروني إلى مجموعة Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a663c-108">**Comments are not getting saved** -  The user adding the comment does not have permission to send email to the Microsoft 365 group.</span></span> <span data-ttu-id="a663c-109">اقرأ [كيف يعمل Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) للحصول على مزيد من المعلومات حول هذا السيناريو.</span><span class="sxs-lookup"><span data-stu-id="a663c-109">Read [How Microsoft Planner Works](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) for more information about this scenario.</span></span>

- <span data-ttu-id="a663c-110">يتم عرض الخطأ **لم يعد لديك حق الوصول**، أو **يتعذر على المستخدمين الضيوف إضافة التعليقات** - قد يرى المستخدمون الضيوف الذين لا يمكنهم إرسال بريد إلكتروني إلى علبة الوارد الخاصة بالمجموعة هذه الرسالة.</span><span class="sxs-lookup"><span data-stu-id="a663c-110">The error **You no longer have access** is displayed, or **guest users are unable to add comments** - Guest users who cannot send e-mail to the group inbox may see this message.</span></span> <span data-ttu-id="a663c-111">لحل هذه المشكلة، تأكد من أن المستخدم الضيف يحتوي على عنوان بريد إلكتروني صالح.</span><span class="sxs-lookup"><span data-stu-id="a663c-111">To resolve, ensure that the guest user has a valid e-mail address.</span></span>

- <span data-ttu-id="a663c-112">**يتلقى المستخدمون الذين تمت إزالتهم رسائل بريد إلكتروني** - إذا علّق مستخدم على مهمة قبل إزالته من الخطة، فإن سلسلة رسائل البريد الإلكتروني تتضمن المستخدم لكل تعليق يتم إجراؤه على المهمة.</span><span class="sxs-lookup"><span data-stu-id="a663c-112">**Removed users are getting emails** -  If a user comments on a task prior to being removed from the plan, the email thread includes the user for each comment made on the task.</span></span>

<span data-ttu-id="a663c-113">للحصول على معلومات تفصيلية حول التعليقات باستخدام Microsoft Planner، راجع [كيفية عمل Microsoft Planner](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) و [التعليق على المهام في Microsoft Planner](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1).</span><span class="sxs-lookup"><span data-stu-id="a663c-113">For detailed information on comments with Microsoft Planner, see [how Microsoft Planner works](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) and [Comment on tasks in Microsoft Planner](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1).</span></span>
