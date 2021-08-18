---
title: التحقق من جميع أنشطة المستخدمين
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332330"
---
# <a name="investigate-all-the-users-activities"></a>التحقق من جميع أنشطة المستخدمين

فيما يلي كيفية القيام بذلك:

1. اتخاذ أحد الإجراءات التالية:
   - في مركز التوافق في Microsoft 365 في <https://compliance.microsoft.com> ، انتقل إلى تدقيق  \> **الحلول**. أو، انتقل مباشرة إلى صفحة **التدقيق،** استخدم <https://compliance.microsoft.com/auditlogsearch> .
   - في مدخل Microsoft 365 Defender في <https://security.microsoft.com> ، انتقل إلى **تدقيق**. أو، انتقل مباشرة إلى صفحة **التدقيق،** استخدم <https://security.microsoft.com/auditlogsearch> .

    **ملاحظة:** إذا رأيت إشعارا بحاجتك إلى تشغيل الميزة، فانتقل إلى الأمام ثم قم ب تشغيلها الآن. إذا لم يتم تشغيل الميزة، فلن تتمكن نتائج البحث من سحب البيانات من التواريخ السابقة.

2. على علامة **التبويب** بحث في **صفحة التدقيق،** قم بتكوين الإعدادات التالية:
   - **نطاق التاريخ والوقت**: حدد نطاق التاريخ/الوقت في **مربعي** البدء **والنهي.**
   - **الأنشطة**: إذا كنت مهتما بنشاط معين، فحدده من القائمة؛ وإلا، فإن القيمة الافتراضية **إظهار النتائج لكل الأنشطة** ترجع كل الأنشطة.
   - **المستخدمون**: اقبل القيمة الافتراضية الفارغة لإرجاع نتائج لجميع المستخدمين، أو أدخل مستخدما واحدا أو أكثر.

3. عند الانتهاء، انقر فوق **بحث**. تظهر الأنشطة على صفحة البحث **الجديدة في التدقيق.** سترى عنوان **IP والمستخدم** **واسم** **النشاط.**

4. لتنزيل النتائج، حدد **تصدير** \> **تنزيل كل النتائج**.

5. حدد نشاطا في النتائج لفتح المعلومات من خلال المعلومات.

لمعرفة المزيد، راجع [البحث في سجل التدقيق للتحقق من مشاكل الدعم الشائعة](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
