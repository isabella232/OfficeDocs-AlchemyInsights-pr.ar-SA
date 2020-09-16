---
title: S/MIME في Outlook علي الويب
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
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772249"
---
# <a name="encrypt-email-messages-in-outlook"></a>تشفير رسائل البريد الكتروني في Outlook

يتم إنشاء تشفير رسائل microsoft 365 علي Microsoft Azure Rights Management (Azure RMS) ، وهو جزء من حماية البيانات في Azure. إذا كان اشتراكك يتضمن أداره الحقوق ل azure أو حماية معلومات Azure ، فلا **تحتاج إلى اتخاذ اي إجراءات لتمكين خدمه أداره الحقوق يدويا أو تنشيطها** .

بالاستناد إلى ملاحظات العملاء ، لن يعود بحاجه إلى تمكين قواعد تدفقات البريد في Exchange لتشفير البريد الكتروني الصادر الذي يحتوي علي نوع معين من المعلومات الحساسة بشكل افتراضي. بدلا من ذلك ، نقدم إرشادات مفصله حول كيفيه القيام بذلك طفرة. للحصول علي مزيد من التفاصيل حول كيفيه إنشاء قاعده نقل لتشفير المعلومات الحساسة ، راجع [هذه المقالة](https://aka.ms/OmeEtr).

- إذا كنت تستخدم Outlook علي الويب (المعروف سابقا باسم **OWA**): عند إنشاء رسالة بريد الكتروني ، ما عليك سوي النقر فوق **حماية** في OWA. سيؤدي ذلك إلى تطبيق الاذن "عدم أعاده التوجيه". انقر فوق **تغيير الاذن** واختر **تشفير** لتشفير الرسالة فقط.

- إذا كنت تستخدم **outlook client**: لإرسال رسالة مشفره من outlook 2013 أو 2016 ، أو Outlook 2016 for Mac ، حدد **الخيارات**  >  **الأذونات**، ثم حدد خيار الحماية الذي تريده.

- **لتشفير كل رسائل البريد الكتروني** التي يتم إرسالها إلى مستلمين معينين أو مؤسسات شركاء خارجيه ، يجب إنشاء قاعده نقل تدفق البريد في مركز أداره Exchange. يتم توفير الإرشادات المفصلة في [مقاله الدعم هذه](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

