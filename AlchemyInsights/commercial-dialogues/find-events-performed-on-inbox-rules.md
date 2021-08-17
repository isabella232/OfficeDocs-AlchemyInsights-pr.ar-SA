---
title: البحث عن الأحداث التي تم تنفيذها على قواعد علبة الوارد
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
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882622"
---
# <a name="find-events-performed-on-inbox-rules"></a>البحث عن الأحداث التي تم تنفيذها على قواعد علبة الوارد

عند إنشاء قواعد علبة الوارد أو تغييرها أو حذفها، يتم تسجيل الأحداث في سجل التدقيق. فيما يلي كيفية مراجعتها:

1. اتخاذ أحد الإجراءات التالية:
   - في مركز التوافق في Microsoft 365 في <https://compliance.microsoft.com> ، انتقل إلى تدقيق  \> **الحلول**. أو، انتقل مباشرة إلى صفحة **التدقيق،** استخدم <https://compliance.microsoft.com/auditlogsearch> .
   - في Microsoft 365 Defender في ، <https://security.microsoft.com> انتقل إلى **تدقيق**. أو، انتقل مباشرة إلى صفحة **التدقيق،** استخدم <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > إذا رأيت إشعارا بحاجتك إلى تشغيل التدقيق، فانتقل إلى وضع تشغيلها الآن. إذا لم يتم تشغيل هذه الميزة، فلن تتمكن نتائج البحث من سحب البيانات من التواريخ السابقة.

2. على علامة **التبويب** بحث في **صفحة التدقيق،** قم بتكوين الإعدادات التالية:
   - **نطاق التاريخ والوقت**: حدد نطاق التاريخ/الوقت في **مربعي** البدء **والنهي.**
   - **الأنشطة**: حدد **New-InboxRule إنشاء** قاعدة علبة الوارد من Outlook Web App

3. عند الانتهاء، انقر فوق **بحث**. تظهر الأنشطة على صفحة البحث **الجديدة في التدقيق.**

4. حدد نشاطا في النتائج لفتح المعلومات من خلال المعلومات. ضمن المقطع **معلمات،** يمكنك رؤية اسم القاعدة والشروط التي تم تعيينها والإجراءات التي ستتخذها القاعدة.

لمعرفة المزيد، راجع [البحث في سجل التدقيق للتحقق من مشاكل الدعم الشائعة](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
