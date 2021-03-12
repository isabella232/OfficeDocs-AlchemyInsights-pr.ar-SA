---
title: إصلاح نهج المستأجر (تجاوز الإجراء)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743077"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="3474b-102">إصلاح نهج المستأجر (تجاوز الإجراء)</span><span class="sxs-lookup"><span data-stu-id="3474b-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="3474b-103">لقد تأثر نهج مكافحة البريد العشوائي في المستأجر بهذه الرسالة.</span><span class="sxs-lookup"><span data-stu-id="3474b-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="3474b-104">لمراجعة النهج، يمكنك القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="3474b-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="3474b-105">انتقل إلى مركز التوافق في [Office 365 security &](https://go.microsoft.com/fwlink/p/?linkid=2077143)، ثم انتقل إلى نهج إدارة المخاطر لمكافحة البريد   >    >  [العشوائي](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="3474b-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="3474b-106">تحقق لمعرفة ما إذا كان **مصدر** النهج يشير إلى ما  **يلي: Add-Xheader/ModifySubject/Redirect/Delete/No action/ رسالة BCC**</span><span class="sxs-lookup"><span data-stu-id="3474b-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="3474b-107">إذا كان الأمر كذلك، على علامة **التبويب** مخصص، تحقق من إعدادات النهج الذي تأثر بالرسالة.</span><span class="sxs-lookup"><span data-stu-id="3474b-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="3474b-108">من المحتمل أن تكون الإعدادات القياسية **المطبقة** على جميع عملاء Exchange Online Protection قد أثرت على الرسالة.</span><span class="sxs-lookup"><span data-stu-id="3474b-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="3474b-109">لمزيد من المعلومات حول تكوين سياسات تصفية البريد العشوائي، راجع [تكوين سياسات](https://go.microsoft.com/fwlink/?linkid=2101431)تصفية البريد العشوائي .</span><span class="sxs-lookup"><span data-stu-id="3474b-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
