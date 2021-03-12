---
title: تشفير بعض رسائل البريد الإلكتروني تلقائيا من office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743113"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="a08bd-102">تشفير بعض رسائل البريد الإلكتروني تلقائيا من office 365</span><span class="sxs-lookup"><span data-stu-id="a08bd-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="a08bd-103">من مركز [إدارة Exchange،](https://outlook.office365.com/ecp/)اختر **تدفق البريد > قواعد .**</span><span class="sxs-lookup"><span data-stu-id="a08bd-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="a08bd-104">انقر فوق **الأيقونة جديد (+)،** ثم انقر فوق تطبيق تشفير الرسائل وحماية الحقوق في **Office 365 على الرسائل.**</span><span class="sxs-lookup"><span data-stu-id="a08bd-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="a08bd-105">في **الاسم**، أدخل اسما للقاعدة، مثل *تشفير كل الرسائل.*</span><span class="sxs-lookup"><span data-stu-id="a08bd-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="a08bd-106">في **تطبيق هذه القاعدة إذا**، اختر **[تطبيق على كل الرسائل]**.</span><span class="sxs-lookup"><span data-stu-id="a08bd-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="a08bd-107">إلى بجانب الحقل **قم بما يلي،** انقر **فوق تحديد واحد**.</span><span class="sxs-lookup"><span data-stu-id="a08bd-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="a08bd-108">في القائمة **المنسدلة قالب RMS،** حدد **تشفير**، ثم انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="a08bd-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="a08bd-109">(إذا لم تشاهد هذا الخيار، فهذا يعني أن خطتك لا تتضمن التشفير التلقائي.</span><span class="sxs-lookup"><span data-stu-id="a08bd-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="a08bd-110">ولكن يمكنك إضافته!)</span><span class="sxs-lookup"><span data-stu-id="a08bd-110">But you can add it!)</span></span>
7. <span data-ttu-id="a08bd-111">حدد **خانة الاختيار تدقيق هذه القاعدة بمستوى الخطورة،** ثم حدد المستوى المطلوب.</span><span class="sxs-lookup"><span data-stu-id="a08bd-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="a08bd-112">إذا كانت شركتك لديها التزامات تعاقدية بإرسال كل رسائل البريد الإلكتروني المشفرة، فإني أوصي بإعداد المستوى إلى **مرتفع.**</span><span class="sxs-lookup"><span data-stu-id="a08bd-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="a08bd-113">ضمن **اختيار نموذج لهذه القاعدة،** انقر فوق **فرض**.</span><span class="sxs-lookup"><span data-stu-id="a08bd-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="a08bd-114">اختر أي تحديد اختياري (من قائمة التحديدات الاختيارية التي يمكنك إجراءها في هذه المرحلة، ويمكن ترك العديد منها مع الإعداد الافتراضي للتبسيط).</span><span class="sxs-lookup"><span data-stu-id="a08bd-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="a08bd-115">انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="a08bd-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a08bd-116">يمكنك دائما الرجوع وتحرير هذه القاعدة لاحقا.</span><span class="sxs-lookup"><span data-stu-id="a08bd-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="a08bd-117">لمزيد من المعلومات حول إنشاء قواعد التشفير، راجع تعريف قواعد تدفق البريد لتشفير رسائل البريد الإلكتروني [في Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="a08bd-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

