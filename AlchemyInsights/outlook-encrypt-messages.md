---
title: S/MIME في Outlook على الويب
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752847"
---
# <a name="encrypt-email-messages-in-outlook"></a>تشفير رسائل البريد الإلكتروني في أوتلوك

تم إنشاء تشفير الرسائل Office 365 على إدارة حقوق Microsoft Azure (Azure RMS)، وهو جزء من حماية معلومات Azure. إذا كان اشتراكك يتضمن إدارة حقوق Azure أو حماية معلومات Azure، **فلن تحتاج إلى اتخاذ أية إجراءات لتمكين أو تنشيط** خدمة إدارة الحقوق يدويًا.

استنادًا إلى ملاحظات العملاء، لن نتمكن بعد الآن من تمكين قواعد تدفق بريد Exchange من تشفير البريد الإلكتروني الصادر تلقائيًا الذي يحتوي على نوع معين من المعلومات الحساسة في المستأجر بشكل افتراضي. بدلا من ذلك، نحن نقدم تعليمات مفصلة حول كيف يمكنك أن تفعل ذلك أنفسكم. للحصول على تفاصيل إضافية حول كيفية إنشاء قاعدة نقل لتشفير المعلومات الحساسة، راجع [هذه المقالة](https://aka.ms/OmeEtr).

- في حالة استخدام Outlook على **** ويب (OWA سابقاً): عند إنشاء رسالة بريد إلكتروني، ببساطة انقر فوق **حماية** في OWA. سيؤدي هذا إلى تطبيق إذن "عدم إعادة توجيه". انقر فوق **تغيير الإذن** واختر **تشفير** لتشفير الرسالة فقط.

- في حالة استخدام **عميل Outlook**: لإرسال رسالة مشفرة من Outlook 2013 أو 2016، أو Outlook 2016 لنظام التشغيل Mac، حدد**أذونات** **الخيارات** > ، ثم حدد خيار الحماية التي تحتاجها.

- لتشفير كافة **رسائل البريد الإلكتروني** المرسلة إلى مستلمين معينين أو المؤسسات الشريكة الخارجية تلقائياً، تحتاج إلى إنشاء قاعدة نقل تدفق بريد في مركز مسؤول Exchange. يتم توفير تعليمات مفصلة في [هذه المقالة الدعم](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

