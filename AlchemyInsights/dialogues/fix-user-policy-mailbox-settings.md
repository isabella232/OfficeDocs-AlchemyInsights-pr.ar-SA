---
title: إصلاح إعدادات نهج المستخدم/علبة البريد
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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692513"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="6462b-102">إصلاح إعدادات نهج المستخدم/علبة البريد</span><span class="sxs-lookup"><span data-stu-id="6462b-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="6462b-103">أثرت إعدادات البريد غير الهام في علبة البريد على هذه الرسالة.</span><span class="sxs-lookup"><span data-stu-id="6462b-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="6462b-104">لمراجعة الإعدادات، يمكنك القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="6462b-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="6462b-105">تشغيل Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="6462b-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="6462b-106">لمزيد من المعلومات، [راجع فتح Exchange Management Shell.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="6462b-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="6462b-107">تشغيل هذا الأمر (باستخدام عنوان البريد الإلكتروني الخاص بالمستخدم):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="6462b-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="6462b-108">تحقق مما إذا كان عنوان البريد الإلكتروني للمرسل جزءا من **TrustedSendersAndDomains** أو **BlockedSendersAndDomains.**</span><span class="sxs-lookup"><span data-stu-id="6462b-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="6462b-109">إذا كان عنوان البريد الإلكتروني في إحدى القوائم، فقد تحتاج إلى إزالته.</span><span class="sxs-lookup"><span data-stu-id="6462b-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="6462b-110">لمعرفة المزيد، راجع [Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)</span><span class="sxs-lookup"><span data-stu-id="6462b-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
