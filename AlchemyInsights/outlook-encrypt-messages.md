---
title: S/MIME في Outlook على ويب
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666827"
---
# <a name="encrypt-email-messages-in-outlook"></a>تشفير رسائل البريد الإلكتروني في Outlook

تشفير الرسائل office 365 تستند إلى Microsoft Azure إدارة الحقوق (RMS Azure)، التي جزء من حماية معلومات Azure. إذا كان يتضمن الاشتراك Azure إدارة حقوق أو حماية المعلومات أزور، **لا تحتاج إلى اتخاذ أي إجراءات لتمكين يدوياً أو تنشيط** "خدمة إدارة الحقوق".

بناء على ملاحظات العملاء، أننا سوف لا يمكن تمكين Exchange قواعد تدفق البريد تلقائياً تشفير البريد الإلكتروني الصادر التي تحتوي على نوع معين من المعلومات الحساسة في المستأجر الخاص بك بشكل افتراضي. بدلاً من ذلك، نقدم إرشادات مفصلة حول كيفية القيام بذلك أنفسكم. للحصول على تفاصيل إضافية حول كيفية إنشاء قاعدة نقل لتشفير المعلومات الحساسة، راجع [هذا المقال](https://aka.ms/OmeEtr).

- في حالة استخدام Outlook على الويب (سابقا **OWA**): عند إنشاء رسالة بريد إلكتروني، ببساطة انقر فوق **حماية** في OWA. سيتم تطبيق هذا الإذن "القيام بإعادة التوجيه". انقر فوق **تغيير الإذن** واختر **تشفير** تشفير الرسالة فقط.

- في حالة استخدام **عميل Outlook**: لإرسال رسالة مشفرة من Outlook 2013 أو 2016 أو Outlook 2016 لنظام التشغيل Mac، قم بتحديد **خيارات** > **الأذونات**، ثم قم بتحديد خيار الحماية التي تحتاجها.

- **تشفير كافة رسائل البريد الإلكتروني** المرسلة إلى بعض المستلمين أو المنظمات الشريكة الخارجية، تحتاج إلى إنشاء قاعدة نقل تدفق بريد في مركز مسؤول Exchange. يتم توفير إرشادات مفصلة في [هذه المقالة الدعم](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

