---
title: تحديد إعادة توجيه بريد إلكتروني خارجي على علب البريد الموجودة في سجلات التدقيق
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539088"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>تحديد متى يتم تكوين إعادة توجيه البريد الإلكتروني الخارجي على علب البريد

عند تكوين مستخدم Office 365 إعادة توجيه البريد الإلكتروني الخارجي على علبة بريد، يتم تدوين النشاط كجزء من cmdlet **مجموعة-علبة البريد** . يمكنك مشاهدة النشاط باستخدام البحث سجل التدقيق في & أمان مركز التوافق.

1. تسجيل الدخول إلى [مركز التوافق & الأمن 365 Office](https://protection.office.com/).

2. انتقل إلى **بحث** > صفحة**البحث في سجل التدقيق** .

3. حدد نطاق التواريخ في حقول **تاريخ البدء** **وتاريخ الانتهاء** . لا تحتاج إلى تحديد اسم مستخدم. تحقق من تعيين حقل **الأنشطة** **إظهار النتائج لكافة الأنشطة**.

4. انقر فوق **بحث**.

في النتائج، انقر فوق **عامل تصفية النتائج** واكتب **علبة مجموعة** في المربع النشاط. حدد سجل تدقيق في النتائج. في القائمة الفرعية **تفاصيل** ، انقر فوق **مزيد من المعلومات**. يجب عليك مراجعة تفاصيل كل سجل التدوين لتحديد حالة تتعلق بالنشاط إرسال البريد الإلكتروني.

- **ObjectId**: قيمة الاسم المستعار علبة البريد التي تم تعديلها.

- **المعلمات**: _فورواردينجسمتبادريس_ يشير إلى عنوان البريد الإلكتروني الهدف.

- **اسم المستخدم**: المستخدم الذي قام بتكوين إعادة توجيه البريد الإلكتروني في صندوق البريد في ميدان **ObjectId** .

لمزيد من المعلومات، راجع [تحديد الذي قام بإعداد علبة بريد إرسال البريد الإلكتروني](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
