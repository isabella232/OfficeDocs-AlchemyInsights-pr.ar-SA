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
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523314"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="22130-102">تشفير بعض رسائل البريد الإلكتروني في Office 365 تلقائيا</span><span class="sxs-lookup"><span data-stu-id="22130-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="22130-103">يمكنك تشفير الرسائل التي يرسلها المستخدمون تلقائيا إلى أشخاص أو مؤسسات خارجية معينة.</span><span class="sxs-lookup"><span data-stu-id="22130-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="22130-104">للقيام بذلك، تنفيذ الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="22130-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="22130-105">من مركز [إدارة Exchange،](https://outlook.office365.com/ecp/)اختر **قواعد > البريد.**</span><span class="sxs-lookup"><span data-stu-id="22130-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="22130-106">انقر فوق **الأيقونة الجديدة (+)،** ثم انقر فوق "تطبيق تشفير الرسائل وحماية الحقوق في **Office 365" على الرسائل.**</span><span class="sxs-lookup"><span data-stu-id="22130-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="22130-107">في **الاسم،** أدخل اسما للقاعدة، مثل *تشفير الرسائل المرسلة* إلى DrToniRamos@gmail.com.</span><span class="sxs-lookup"><span data-stu-id="22130-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="22130-108">في **تطبيق هذه القاعدة إذا**، اختر المستلم > هذا **الشخص.**</span><span class="sxs-lookup"><span data-stu-id="22130-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="22130-109">في النافذة **"تحديد الأعضاء"،** حدد اسم الشخص الذي تريد تطبيق قاعدة التشفير عليه، ثم انقر فوق **"إضافة".**</span><span class="sxs-lookup"><span data-stu-id="22130-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="22130-110">عندما تنتهي من إضافة المستخدمين، انقر فوق **"موافق".**</span><span class="sxs-lookup"><span data-stu-id="22130-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="22130-111">بجانب الحقل **"قم بما يلي"،** انقر فوق **"تحديد واحد".**</span><span class="sxs-lookup"><span data-stu-id="22130-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="22130-112">في القائمة المنسدلة **قالب RMS،** حدد **"تشفير"،** ثم انقر فوق **"موافق".**</span><span class="sxs-lookup"><span data-stu-id="22130-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="22130-113">(إذا لم تشاهد هذا الخيار، فهذا يعني أن خطتك لا تتضمن تشفيرا تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="22130-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="22130-114">ولكن يمكنك إضافته!)</span><span class="sxs-lookup"><span data-stu-id="22130-114">But you can add it!)</span></span>
9. <span data-ttu-id="22130-115">اختر أي تحديد اختياري (من قائمة التحديدات الاختيارية التي يمكنك إجراءها في هذه المرحلة، والكثير منها يمكن تركه مع الإعداد الافتراضي للتبسيط).</span><span class="sxs-lookup"><span data-stu-id="22130-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="22130-116">انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="22130-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="22130-117">يمكنك دائما الرجوع وتحرير هذه القاعدة لاحقا.</span><span class="sxs-lookup"><span data-stu-id="22130-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="22130-118">لمزيد من المعلومات حول إنشاء قواعد التشفير، راجع تعريف قواعد تدفق البريد لتشفير رسائل البريد الإلكتروني [في Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="22130-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

