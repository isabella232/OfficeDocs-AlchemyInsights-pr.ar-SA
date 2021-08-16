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
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028711"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>تحديد وقت تكوين إعادة توجيه البريد الإلكتروني الخارجي على علب البريد

عندما يقوم Microsoft 365 بتكوين إعادة توجيه البريد الإلكتروني الخارجي في علبة بريد، يتم تدقيق النشاط كجزء من الأمر **cmdlet الخاص** بتعيين علبة البريد. يمكنك رؤية النشاط باستخدام البحث في سجل التدقيق في مركز & الأمان.

1. سجل دخولك إلى Microsoft 365 [التوافق.](https://protection.office.com/)

2. انتقل إلى صفحة **البحث**  >  **في سجل تدقيق** البحث.

3. حدد نطاق التاريخ في **حقلي تاريخ البدء** **وتاريخ** الانتهاء. لست بحاجة إلى تحديد اسم مستخدم. تحقق من **تعيين** الحقل الأنشطة إلى **إظهار النتائج لكل الأنشطة**.

4. انقر **فوق بحث**.

في النتائج، انقر فوق **تصفية النتائج** وا اكتب **Set-Mailbox** في مربع عامل تصفية النشاط. حدد سجل تدقيق في النتائج. في **منتهى التفاصيل،** انقر فوق **مزيد من المعلومات**. يجب عليك النظر في تفاصيل كل سجل تدقيق لتحديد ما إذا كان النشاط مرتبطا ب إعادة توجيه البريد الإلكتروني.

- **ObjectId**: القيمة المستعارة لعلبة البريد التي تم تعديلها.

- **المعلمات:** _تشير إعادة توجيهSmtpAddress إلى_ عنوان البريد الإلكتروني الهدف.

- **UserId**: المستخدم الذي قام بتكوين إعادة توجيه البريد الإلكتروني على علبة البريد في **حقل ObjectId.**

لمزيد من المعلومات، راجع تحديد من قام بإعداد إعادة توجيه [البريد الإلكتروني لعلبة بريد](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
