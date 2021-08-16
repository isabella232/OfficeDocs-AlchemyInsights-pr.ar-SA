---
title: S/MIME في Outlook على ويب
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010711"
---
# <a name="encrypt-email-messages-in-outlook"></a>تشفير رسائل البريد الإلكتروني في Outlook

Microsoft 365 تم بناء تشفير الرسائل على Microsoft Azure Rights Management (Azure RMS)، الذي هو جزء من Azure Information Protection. إذا كان اشتراكك يتضمن Azure Rights  Management أو Azure Information Protection، لست بحاجة إلى اتخاذ أي إجراءات لتمكين خدمة إدارة الحقوق أو تنشيطها يدويا.

استنادا إلى ملاحظات العملاء، لن يمكننا بعد الآن Exchange قواعد تدفق البريد لتشفير البريد الإلكتروني الصادر الذي يحتوي على نوع معين من المعلومات الحساسة في المستأجر بشكل افتراضي. بدلا من ذلك، نحن نقدم إرشادات مفصلة حول كيفية القيام بذلك بنفسك. للحصول على تفاصيل إضافية حول كيفية إنشاء قاعدة نقل لتشفير المعلومات الحساسة، راجع [هذه المقالة](https://aka.ms/OmeEtr).

- إذا كنت Outlook على الويب (سابقا **OWA):** عند إنشاء رسالة بريد إلكتروني، انقر ببساطة فوق **حماية** في OWA. سيطبق هذا الإذن "عدم إعادة توجيه". انقر **فوق تغيير الإذن** **واختر تشفير** لتشفير الرسالة فقط.

- إذا كنت **تستخدم Outlook**: لإرسال رسالة مشفرة من Outlook 2013 أو 2016 أو Outlook 2016 for Mac، حدد خيارات الأذونات ، ثم حدد خيار الحماية الذي  >  تحتاجه.

- **لتشفير كل رسائل** البريد الإلكتروني المرسلة تلقائيا إلى مستلمين معينين أو مؤسسات شريكة خارجية، ستحتاج إلى إنشاء قاعدة نقل تدفق البريد في Exchange الإدارة. يتم توفير إرشادات مفصلة في [مقالة الدعم هذه](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

