---
title: قراءة سجلات التدقيق للأحداث المحذوفة
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
ms.openlocfilehash: ef4cbb0b778b22fba83d22d5056449c2281c5a2947ecb41ce8f808a4d1132426
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896002"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>قراءة سجلات التدقيق للأحداث المحذوفة

فيما يلي كيفية القيام بذلك:

1. اتخاذ أحد الإجراءات التالية:
   - في مركز التوافق في Microsoft 365 في <https://compliance.microsoft.com> ، انتقل إلى تدقيق  \> **الحلول**. أو، انتقل مباشرة إلى صفحة **التدقيق،** استخدم <https://compliance.microsoft.com/auditlogsearch> .
   - في مدخل Microsoft 365 Defender في <https://security.microsoft.com> ، انتقل إلى **تدقيق**. أو، انتقل مباشرة إلى صفحة **التدقيق،** استخدم <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > إذا رأيت إشعارا بأنه يجب تشغيل الميزة، فانتقل إلى تشغيلها الآن. إذا لم يتم تشغيل الميزة، فلن تتمكن نتائج البحث من سحب البيانات من التواريخ السابقة.

2. على علامة **التبويب** بحث في **صفحة التدقيق،** قم بتكوين الإعدادات التالية:
   - **نطاق التاريخ والوقت**: حدد نطاق التاريخ/الوقت في **مربعي** البدء **والنهي.**
   - **الأنشطة**: **أدخل Exchange علبة البريد** ثم حدد القيم التالية:
     - **الرسائل المحذوفة من مجلد "العناصر المحذوفة"**
     - **الرسائل التي تم نقلها إلى مجلد "العناصر المحذوفة"**

       عندما تنتهي، انقر خارج الجزء لتصغير **جزء** الأنشطة.

   - **المستخدمون**: اقبل القيمة الافتراضية الفارغة لإرجاع نتائج لجميع المستخدمين، أو أدخل مستخدما واحدا أو أكثر.

3. عند الانتهاء، انقر فوق **بحث**. تظهر الأنشطة على صفحة البحث **الجديدة في التدقيق.**

4. حدد نشاطا في النتائج لفتح المعلومات من خلال المعلومات. يتم عرض معلومات إضافية حول العنصر المحذوف، مثل سطر الموضوع وموقع العنصر عند حذفه، في الحقل **AffectedItems.**

   > [!NOTE]
   > لا يمكنك استعادة العناصر المحذوفة باستخدام ميزة سجل التدقيق. لاستعادة العناصر المحذوفة، راجع استرداد رسائل البريد الإلكتروني [المحذوفة في Outlook على ويب](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

لمزيد من المعلومات، راجع [البحث في سجل التدقيق للتحقق من مشاكل الدعم الشائعة](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
