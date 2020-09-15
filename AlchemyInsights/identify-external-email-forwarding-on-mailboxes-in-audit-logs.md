---
title: تحديد أعاده توجيه البريد الكتروني الخارجي علي علب البريد في سجلات التدقيق
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696284"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>تحديد وقت تكوين أعاده توجيه البريد الكتروني الخارجي علي علب البريد

عند قيام مستخدم Microsoft 365 بتكوين أعاده توجيه البريد الكتروني الخارجي علي علبه البريد ، يتم تدقيق النشاط كجزء من الأمر cmdlet **علبه البريد** . يمكنك رؤية النشاط باستخدام البحث في سجل التدقيق في مركز توافق & الأمان.

1. سجل الدخول إلى [مركز توافق & أمان Microsoft 365](https://protection.office.com/).

2. انتقل إلى صفحه **Search**  >  **البحث في سجل تدقيق** البحث.

3. حدد نطاق التاريخ في الحقلين **"تاريخ البدء** " و " **تاريخ الانتهاء** ". لا تحتاج إلى تحديد اسم المستخدم. تاكد من تعيين الحقل " **الانشطه** " **لعرض النتائج لكل الانشطه**.

4. انقر فوق **بحث**.

في النتائج ، انقر فوق **تصفيه النتائج** واكتب **Set-علبه البريد** في المربع عامل تصفيه النشاط. حدد سجل تدقيق في النتائج. في القائمة المنبثقة **التفاصيل** ، انقر فوق **مزيد من المعلومات**. يجب عليك إلقاء نظره علي تفاصيل كل سجل تدقيق لتحديد ما إذا كان النشاط مرتبطا باعاده توجيه البريد الكتروني.

- **ObjectId**: القيمة المستعارة لعلبه البريد التي تم تعديلها.

- **المعلمات**: _فورواردينجسمتبادريس_ تشير إلى عنوان البريد الكتروني الهدف.

- **UserId**: المستخدم الذي قام بتكوين أعاده توجيه البريد الكتروني علي علبه البريد في الحقل **ObjectId** .

لمزيد من المعلومات ، راجع [تحديد الأشخاص الذين قاموا باعداد أعاده توجيه البريد الكتروني لعلبه البريد](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
