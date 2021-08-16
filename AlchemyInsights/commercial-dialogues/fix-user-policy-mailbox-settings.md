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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034705"
---
# <a name="fix-user-policymailbox-settings"></a>إصلاح إعدادات نهج المستخدم/علبة البريد

أثرت إعدادات البريد غير الهام في علبة البريد على هذه الرسالة. لمراجعة الإعدادات، يمكنك القيام بما يلي:

1. تشغيل Exchange Management Shell. لمزيد من المعلومات، راجع [فتح Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. تشغيل هذا الأمر (باستخدام عنوان البريد الإلكتروني الخاص  **بالمستخدم): get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. تحقق مما إذا كان عنوان البريد الإلكتروني للمرسل جزءا من **TrustedSendersAndDomains** أو **BlockedSendersAndDomains**. إذا كان عنوان البريد الإلكتروني في إحدى القوائم، فقد تحتاج إلى إزالته. لمعرفة المزيد، راجع [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
