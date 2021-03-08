---
title: تشفير رسائل بريد Office 365 الإلكتروني المرسلة إلى مجالات معينة تلقائيا
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523310"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="235ce-102">تشفير رسائل بريد Office 365 الإلكتروني المرسلة إلى مجالات معينة تلقائيا</span><span class="sxs-lookup"><span data-stu-id="235ce-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="235ce-103">من مركز [إدارة Exchange،](https://outlook.office365.com/ecp/)اختر **قواعد > البريد.**</span><span class="sxs-lookup"><span data-stu-id="235ce-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="235ce-104">انقر فوق **الأيقونة الجديدة (+)،** ثم انقر فوق "تطبيق تشفير الرسائل وحماية الحقوق في **Office 365" على الرسائل.**</span><span class="sxs-lookup"><span data-stu-id="235ce-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="235ce-105">في **الاسم،** أدخل اسما للقاعدة، مثل *تشفير الرسائل المرسلة إلى* contoso.com.</span><span class="sxs-lookup"><span data-stu-id="235ce-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="235ce-106">في **تطبيق هذه القاعدة إذا**، اختر المستلم > المجال **هو.**</span><span class="sxs-lookup"><span data-stu-id="235ce-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="235ce-107">أدخل اسم المجال، مثل **contoso.com.**</span><span class="sxs-lookup"><span data-stu-id="235ce-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="235ce-108">انقر فوق **الأيقونة إضافة (+)،** ثم انقر فوق **موافق.**</span><span class="sxs-lookup"><span data-stu-id="235ce-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="235ce-109">بجانب الحقل **"قم بما يلي"،** انقر فوق **"تحديد واحد".**</span><span class="sxs-lookup"><span data-stu-id="235ce-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="235ce-110">في القائمة المنسدلة **قالب RMS،** حدد **"تشفير"،** ثم انقر فوق **"موافق".**</span><span class="sxs-lookup"><span data-stu-id="235ce-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="235ce-111">(إذا لم تشاهد هذا الخيار، فهذا يعني أن خطتك لا تتضمن تشفيرا تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="235ce-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="235ce-112">ولكن يمكنك إضافته!)</span><span class="sxs-lookup"><span data-stu-id="235ce-112">But you can add it!)</span></span>
9. <span data-ttu-id="235ce-113">اختر أي تحديد اختياري (من قائمة التحديدات الاختيارية التي يمكنك إجراءها في هذه المرحلة، والكثير منها يمكن تركه مع الإعداد الافتراضي للتبسيط).</span><span class="sxs-lookup"><span data-stu-id="235ce-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="235ce-114">انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="235ce-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="235ce-115">يمكنك دائما الرجوع وتحرير هذه القاعدة لاحقا.</span><span class="sxs-lookup"><span data-stu-id="235ce-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="235ce-116">لمزيد من المعلومات حول إنشاء قواعد للتشفير، راجع "تعريف قواعد تدفق البريد" لتشفير رسائل البريد الإلكتروني [في Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="235ce-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>