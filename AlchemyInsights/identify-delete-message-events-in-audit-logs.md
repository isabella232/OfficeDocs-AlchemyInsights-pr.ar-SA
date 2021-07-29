---
title: تحديد أحداث الرسائل في سجلات التدقيق
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7dd9c98bd45c29702fbc6cc14bf82bf7bce7d89d
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630056"
---
# <a name="audit-logs-for-deleted-email-messages"></a>سجلات التدقيق لرسائل البريد الإلكتروني المحذوفة

بدءا من يناير 2019، تقوم Microsoft ب تشغيل تسجيل تدقيق علبة البريد بشكل افتراضي. وبخلاف ذلك، لمراجعة أحداث حذف الرسائل لمستخدم معين، ستحتاج إلى تمكين إجراءات الحذف للتدقيق يدويا. إذا تم تمكين تسجيل تدقيق علبة البريد لمنظمتك أو للمستخدم المحدد بالفعل، فاتبع الخطوات أدناه.

1. تسجيل الدخول إلى مركز [Microsoft 365 التوافق](https://protection.office.com/)

2. انقر **فوق البحث والتدقيق** وحدد **البحث في سجل التدقيق**.

3. حدد نطاق التاريخ في **حقلي تاريخ البدء** **وتاريخ** الانتهاء. حدد اسم المستخدم للمستخدم الذي تريد التحقق من اسمه (المستخدم الذي حذف العناصر). في الحقل **الأنشطة،** حدد الرسائل **المحذوفة** من مجلد العناصر المحذوفة والرسائل التي تم نقلها إلى **مجلد العناصر المحذوفة**.

4. انقر **فوق بحث**.

في النتائج، حدد سجل تدقيق. في منتهى التفاصيل، انقر فوق **مزيد من المعلومات**. يتم عرض معلومات إضافية حول العنصر المحذوف (على سبيل المثال، سطر الموضوع وموقع العنصر عند حذفه) في الحقل **AffectedItems.** تظهر **الخاصية ClientInfoString** ما إذا كان الحذف قد حدث في Outlook أو Outlook على ويب (المعروف سابقا باسم Outlook Web App) أو أي جهاز آخر.

لمزيد من المعلومات، راجع تحديد من قام بإعداد إعادة توجيه [البريد الإلكتروني لعلبة بريد](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**ملاحظة:** لا يمكنك استرداد العناصر المحذوفة باستخدام ميزة سجل التدقيق. لاسترداد الرسائل المحذوفة في Outlook على ويب، راجع استرداد العناصر المحذوفة [في Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
