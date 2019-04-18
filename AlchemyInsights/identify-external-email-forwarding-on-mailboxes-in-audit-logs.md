---
title: تحديد إعادة توجيه بريد إلكتروني خارجي على علب البريد الموجودة في سجلات التدقيق
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909005"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>تحديد متى يتم تكوين إعادة توجيه البريد الإلكتروني الخارجي على علب البريد

عندما يقوم مستخدم بتكوين إعادة توجيه البريد الإلكتروني الخارجي على علبة بريد، يتم تدوين النشاط كجزء من cmdlet **مجموعة-علبة البريد** . يمكنك مشاهدة النشاط باستخدام البحث سجل التدقيق في & أمان مركز التوافق.

1. تسجيل الدخول إلى [مركز التوافق ل Office الأمن 365 &](https://protection.office.com/)

2. انقر فوق **البحث والتحقيق** ، وحدد **البحث في سجل التدقيق**.

3. حدد نطاق التواريخ في حقول **تاريخ البدء** **وتاريخ الانتهاء** . لا تحتاج إلى تحديد اسم مستخدم. تحقق من تعيين حقل **الأنشطة** **إظهار النتائج لكافة الأنشطة**.

4. انقر فوق **بحث**.

في النتائج، انقر فوق **عامل تصفية النتائج** واكتب **علبة مجموعة** في المربع النشاط. حدد سجل تدقيق في النتائج. في القائمة الفرعية **تفاصيل** ، انقر فوق **مزيد من المعلومات**. يجب عليك مراجعة تفاصيل كل سجل التدوين لتحديد حالة تتعلق بالنشاط إرسال البريد الإلكتروني.

- **ObjectId**: قيمة الاسم المستعار علبة البريد التي تم تعديلها.

- **المعلمات**: _فورواردينجسمتبادريس_ يشير إلى عنوان البريد الإلكتروني الهدف.

- **اسم المستخدم**: المستخدم الذي قام بتكوين إعادة توجيه البريد الإلكتروني في صندوق البريد في ميدان **ObjectId** .

لمزيد من المعلومات، راجع [تحديد الذي قام بإعداد علبة بريد إرسال البريد الإلكتروني](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
