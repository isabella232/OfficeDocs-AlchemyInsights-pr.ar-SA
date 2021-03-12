---
title: تشفير بعض رسائل البريد الإلكتروني في Office 365 تلقائيا
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743112"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="5ad31-102">تشفير بعض رسائل البريد الإلكتروني في Office 365 تلقائيا</span><span class="sxs-lookup"><span data-stu-id="5ad31-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="5ad31-103">يمكنك تشفير الرسائل التي يرسلها المستخدمون تلقائيا إلى أشخاص أو مؤسسات خارجية معينة.</span><span class="sxs-lookup"><span data-stu-id="5ad31-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="5ad31-104">للقيام بذلك، تنفيذ الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="5ad31-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="5ad31-105">من مركز [إدارة Exchange،](https://outlook.office365.com/ecp/)اختر **تدفق البريد > قواعد .**</span><span class="sxs-lookup"><span data-stu-id="5ad31-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="5ad31-106">انقر فوق **الأيقونة جديد (+)،** ثم انقر فوق تطبيق تشفير الرسائل وحماية الحقوق في **Office 365 على الرسائل.**</span><span class="sxs-lookup"><span data-stu-id="5ad31-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="5ad31-107">في **الاسم**، أدخل اسما للقاعدة، مثل *تشفير الرسائل المرسلة إلى DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="5ad31-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="5ad31-108">في **تطبيق هذه القاعدة إذا**، اختر المستلم > هو هذا **الشخص**.</span><span class="sxs-lookup"><span data-stu-id="5ad31-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="5ad31-109">في النافذة **تحديد الأعضاء،** حدد اسم الشخص الذي تريد تطبيق قاعدة التشفير عليه، ثم انقر فوق **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="5ad31-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="5ad31-110">عندما تنتهي من إضافة مستخدمين، انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="5ad31-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="5ad31-111">إلى بجانب الحقل **قم بما يلي،** انقر **فوق تحديد واحد**.</span><span class="sxs-lookup"><span data-stu-id="5ad31-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="5ad31-112">في القائمة **المنسدلة قالب RMS،** حدد **تشفير**، ثم انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="5ad31-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="5ad31-113">(إذا لم تشاهد هذا الخيار، فهذا يعني أن خطتك لا تتضمن التشفير التلقائي.</span><span class="sxs-lookup"><span data-stu-id="5ad31-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="5ad31-114">ولكن يمكنك إضافته!)</span><span class="sxs-lookup"><span data-stu-id="5ad31-114">But you can add it!)</span></span>
9. <span data-ttu-id="5ad31-115">اختر أي تحديد اختياري (من قائمة التحديدات الاختيارية التي يمكنك إجراءها في هذه المرحلة، ويمكن ترك العديد منها مع الإعداد الافتراضي للتبسيط).</span><span class="sxs-lookup"><span data-stu-id="5ad31-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="5ad31-116">انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5ad31-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5ad31-117">يمكنك دائما الرجوع وتحرير هذه القاعدة لاحقا.</span><span class="sxs-lookup"><span data-stu-id="5ad31-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="5ad31-118">لمزيد من المعلومات حول إنشاء قواعد التشفير، راجع تعريف قواعد تدفق البريد لتشفير رسائل البريد الإلكتروني [في Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="5ad31-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

