---
title: تحديد نشاط قاعدة علبة الوارد في سجلات التدقيق
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331110"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>تحديد نشاط قاعدة علبة الوارد في سجلات التدقيق

يمكنك استخدام البحث في سجل التدقيق في مركز التوافق في Microsoft 365 لعرض أحداث قواعد علبة الوارد (إنشاء قواعد علبة الوارد وتعديلها وحذفها).

1. القيام بوا واحدة من الخطوات التالية:
   - في مركز التوافق في Microsoft 365 <https://compliance.microsoft.com> في ، انتقل إلى تدقيق  \> **الحلول**. أو، انتقل مباشرة إلى صفحة **التدقيق،** استخدم <https://compliance.microsoft.com/auditlogsearch> .
   - في مدخل Microsoft 365 Defender في <https://security.microsoft.com> ، انتقل إلى **تدقيق**. أو، انتقل مباشرة إلى صفحة **التدقيق،** استخدم <https://security.microsoft.com/auditlogsearch> .

2. على علامة **التبويب** بحث في **صفحة التدقيق،** قم بتكوين الإعدادات التالية:
   - **نطاق التاريخ والوقت**: حدد نطاق التاريخ/الوقت في **مربعي** البدء **والنهي.**
   - **الأنشطة**: حدد واحدة أو أكثر من القيم التالية:
     - **New-InboxRule إنشاء قاعدة علبة الوارد من Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **تحديث قواعد علبة الوارد من عميل Outlook الوارد**

3. عند الانتهاء، انقر فوق **بحث**. تظهر الأنشطة على صفحة البحث **الجديدة في التدقيق.**

4. حدد نشاطا في النتائج لفتح المعلومات من خلال المعلومات. يتم عرض معلومات حول إعدادات قاعدة علبة الوارد في الحقل **معلمات.**

لمزيد من المعلومات، راجع تحديد ما إذا كان المستخدم قد أنشأ [قاعدة علبة وارد](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
