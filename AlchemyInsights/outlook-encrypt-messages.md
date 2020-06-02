---
title: S / MIME في Outlook على الويب
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511495"
---
# <a name="encrypt-email-messages-in-outlook"></a>تشفير رسائل البريد الإلكتروني في Outlook

تم إنشاء تشفير رسالة Microsoft 365 على Microsoft Azure Rights Management (Azure RMS)، وهو جزء من حماية معلومات Azure. إذا كان اشتراكك يتضمن إدارة حقوق Azure أو حماية معلومات Azure، فلن تحتاج إلى اتخاذ أي إجراءات لتمكين خدمة إدارة الحقوق **أو تنشيطها يدويًا.**

استنادًا إلى ملاحظات العملاء، لن نتمكن بعد الآن من تمكين قواعد تدفق بريد Exchange من تشفير البريد الإلكتروني الصادر تلقائيًا الذي يحتوي على نوع معين من المعلومات الحساسة في المستأجر الخاص بك بشكل افتراضي. وبدلا من ذلك، نقدم تعليمات مفصلة عن كيفية القيام بذلك بأنفسكم. للحصول على تفاصيل إضافية حول كيفية إنشاء قاعدة نقل لتشفير المعلومات الحساسة، راجع [هذه المقالة](https://aka.ms/OmeEtr).

- إذا كنت تستخدم Outlook على الويب **(OWA**سابقاً): عند إنشاء رسالة بريد إلكتروني، ما عليك سوى النقر فوق **حماية** في OWA. سيؤدي ذلك إلى تطبيق إذن "عدم إعادة التوجيه". انقر فوق **تغيير الإذن** واختر **تشفير** لتشفير الرسالة فقط.

- في حالة استخدام **عميل Outlook:** لإرسال رسالة مشفرة من Outlook 2013 أو 2016، أو Outlook 2016 لنظام التشغيل Mac، حدد **أذونات الخيارات،**  >  **Permissions**ثم حدد خيار الحماية الذي تحتاجه.

- لتشفير كافة رسائل البريد الإلكتروني المرسلة **تلقائيًا** إلى مستلمين معينين أو مؤسسات شريكة خارجية، تحتاج إلى إنشاء قاعدة نقل تدفق بريد في مركز Exchange Admin. يتم توفير تعليمات مفصلة في [هذه المقالة الدعم](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

