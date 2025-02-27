---
title: تعرف على الأشخاص الذين قاموا بإعداد إعادة توجيه على علبة بريد، وكيفية
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317795"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>تعرف على الأشخاص الذين قاموا بإعداد إعادة توجيه على علبة بريد، وكيفية

إذا تم تعيين إعادة توجيه خارجية على علبة بريد، فيتم تدقيق النشاط كجزء من **الأمر cmdlet Set-Mailbox.** فيما يلي كيفية العثور على النشاط في سجل التدقيق:

1. اتخاذ أحد الإجراءات التالية:
   - في مركز التوافق في Microsoft 365 <https://compliance.microsoft.com> في ، انتقل إلى تدقيق  \> **الحلول**. أو، انتقل مباشرة إلى صفحة **التدقيق،** استخدم <https://compliance.microsoft.com/auditlogsearch> .
   - في مدخل Microsoft 365 Defender في <https://security.microsoft.com> ، انتقل إلى **تدقيق**. أو، انتقل مباشرة إلى صفحة **التدقيق،** استخدم <https://security.microsoft.com/auditlogsearch> .

   **ملاحظة:** إذا رأيت إشعارا بحاجتك إلى تشغيل التدقيق، فانتقل إلى العمل ثم قم ب تشغيله الآن. إذا لم يتم تشغيل هذه الميزة، فلن تتمكن نتائج البحث من سحب البيانات من التواريخ السابقة.

2. في صفحة **التدقيق،** تحقق  من تحديد علامة التبويب بحث ثم قم بتكوين الإعدادات التالية:
   - حدد نطاق التاريخ/الوقت في **مربعي البدء** **والنهي.**
   - تحقق من **احتواء المربع** الأنشطة على إظهار النتائج **لجميع الأنشطة**.

3. عند الانتهاء، انقر فوق **بحث**. تظهر الأنشطة على صفحة البحث **الجديدة في التدقيق.**

4. في النتائج، انقر فوق العمود **نشاط** لفرز النتائج، وابحث عن إدخالات **Set-Mailbox.**

5. حدد نشاطا في النتائج لفتح المعلومات من خلال المعلومات. ستحتاج إلى مراجعة تفاصيل كل سجل تدقيق لتحديد ما إذا كان النشاط مرتبطا ب إعادة توجيه البريد الإلكتروني:
   - **ObjectId**: القيمة المستعارة لعلبة البريد التي تم تعديلها.
   - **المعلمات:** _تشير إعادة توجيهSmtpAddress إلى_ عنوان البريد الإلكتروني الهدف.
   - **UserId**: المستخدم الذي قام بتكوين إعادة توجيه البريد الإلكتروني على علبة البريد في **حقل ObjectId.**

لمزيد من المعلومات، راجع تحديد من قام بإعداد إعادة توجيه [البريد الإلكتروني لعلبة بريد](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
