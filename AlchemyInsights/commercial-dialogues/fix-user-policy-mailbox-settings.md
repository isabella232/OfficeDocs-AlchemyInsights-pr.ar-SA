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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743392"
---
# <a name="fix-user-policymailbox-settings"></a>إصلاح إعدادات نهج المستخدم/علبة البريد

أثرت إعدادات البريد غير الهام في علبة البريد على هذه الرسالة. لمراجعة الإعدادات، يمكنك القيام بما يلي:

1. تشغيل Exchange Management Shell. لمزيد من المعلومات، [راجع فتح Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. تشغيل هذا الأمر (باستخدام عنوان البريد الإلكتروني الخاص  **بالمستخدم): get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. تحقق مما إذا كان عنوان البريد الإلكتروني للمرسل جزءا من **TrustedSendersAndDomains** أو **BlockedSendersAndDomains**. إذا كان عنوان البريد الإلكتروني في إحدى القوائم، فقد تحتاج إلى إزالته. لمعرفة المزيد، راجع [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
