---
title: تحديد إعادة توجيه البريد الإلكتروني الخارجي على علب البريد في سجلات التدقيق
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331146"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>تحديد وقت تكوين إعادة توجيه البريد الإلكتروني الخارجي على علب البريد

عندما يقوم Microsoft 365 بتكوين إعادة توجيه البريد الإلكتروني الخارجي على علبة بريد، يتم تدقيق النشاط كجزء من الأمر **cmdlet الخاص** بتعيين علبة البريد. يمكنك رؤية النشاط باستخدام البحث في سجل التدقيق. إليك كيفية القيام بذلك.

1. القيام بوا واحدة من الخطوات التالية:
   - في مركز التوافق في Microsoft 365 <https://compliance.microsoft.com> في ، انتقل إلى تدقيق  \> **الحلول**. أو، انتقل مباشرة إلى صفحة **التدقيق،** استخدم <https://compliance.microsoft.com/auditlogsearch> .
   - في مدخل Microsoft 365 Defender في <https://security.microsoft.com> ، انتقل إلى **تدقيق**. أو، انتقل مباشرة إلى صفحة **التدقيق،** استخدم <https://sip.security.microsoft.com/auditlogsearch> .

2. في صفحة **التدقيق،** تحقق  من تحديد علامة التبويب بحث ثم قم بتكوين الإعدادات التالية:
   - حدد نطاق التاريخ/الوقت في **مربعي البدء** **والنهي.**
   - تحقق من **احتواء المربع** الأنشطة على إظهار النتائج **لجميع الأنشطة**.

3. عند الانتهاء، انقر فوق **بحث**. تظهر الأنشطة على صفحة البحث **الجديدة في التدقيق.**

4. في النتائج، انقر فوق **تصفية النتائج** وا اكتب **Set-Mailbox** في مربع عامل تصفية النشاط.

5. حدد سجل تدقيق في النتائج. في **منتهى التفاصيل،** انقر فوق **مزيد من المعلومات**. يجب عليك النظر في تفاصيل كل سجل تدقيق لتحديد ما إذا كان النشاط مرتبطا ب إعادة توجيه البريد الإلكتروني.

   - **ObjectId**: القيمة المستعارة لعلبة البريد التي تم تعديلها.
   - **المعلمات:** _تشير إعادة توجيهSmtpAddress إلى_ عنوان البريد الإلكتروني الهدف.
   - **UserId**: المستخدم الذي قام بتكوين إعادة توجيه البريد الإلكتروني على علبة البريد في **حقل ObjectId.**

لمزيد من المعلومات، راجع تحديد من قام بإعداد إعادة توجيه [البريد الإلكتروني لعلبة بريد](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
