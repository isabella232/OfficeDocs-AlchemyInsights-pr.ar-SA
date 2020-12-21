---
title: أجريجاتيجروبمايلبوكس NDR التي تم تلقيها للبريد الكتروني المرسل إلى مجموعه Microsoft 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/18/2020
ms.locfileid: "49721745"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>أجريجاتيجروبمايلبوكس NDR التي تم تلقيها للبريد الكتروني المرسل إلى مجموعه Microsoft 365

استخدم الأمر التالي أكسو Shell لإنشاء قاعده نقل Exchange لإسقاط رسائل البريد الكتروني التي تم إرسالها إلى علبه بريد المجموعة المجمعة بدون مطالبه:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> استبدل عنوان SMTP في **سينتو** بعنوان smtp الخاص بعلبه بريد المجموعة التجميعية في نطاق المستاجر. يمكنك الحصول علي عنوان SMTP لعلبه بريد المجموعة التجميعية من NDR التي تم تلقيها.



