---
title: تحديد احداث الرسائل التي تم حذفها في سجلات التدقيق
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
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696500"
---
# <a name="audit-logs-for-deleted-email-messages"></a>سجلات التدقيق لرسائل البريد الكتروني المحذوفة

بدءا من يناير 2019 ، فان Microsoft سيقوم بتشغيل تسجيل تدقيق علبه البريد بشكل افتراضي. وبخلاف ذلك ، لمراجعه احداث الرسائل التي تم حذفها لمستخدم معين ، تحتاج إلى تمكين إجراءات الحذف يدويا. إذا كان تسجيل تدقيق علبه البريد ممكنا لمؤسسك أو لمستخدم معين ، فاتبع الخطوات أدناه.

1. تسجيل الدخول إلى [مركز توافق & أمان Microsoft 365](https://protection.office.com/)

2. انقر فوق **البحث والاستقصاء** وحدد **البحث في سجل التدقيق**.

3. حدد نطاق التاريخ في الحقلين **"تاريخ البدء** " و " **تاريخ الانتهاء** ". حدد اسم المستخدم للمستخدم الذي تريد التحقق منه (المستخدم الذي حذف العناصر). في حقل **الانشطه** ، حدد **الرسائل المحذوفة من مجلد العناصر المحذوفة** **ونقل الرسائل إلى مجلد العناصر المحذوفة**.

4. انقر فوق **بحث**.

في النتائج ، حدد سجل تدقيق. في القائمة المنبثقة التفاصيل ، انقر فوق **مزيد من المعلومات**. يتم عرض معلومات اضافيه حول العنصر المحذوف (علي سبيل المثال ، سطر الموضوع وموقع العنصر عند حذفه) في الحقل **أفيكتيديتيمس** . ستظهر الخاصية **كلينتينفوسترينج** إذا حدث الحذف في Outlook أو outlook علي الويب (المعروف سابقا ب Outlook web App) أو اي جهاز آخر.

لمزيد من المعلومات ، راجع [تحديد الأشخاص الذين قاموا باعداد أعاده توجيه البريد الكتروني لعلبه البريد](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**ملاحظه**: لا يمكنك استرداد العناصر المحذوفة باستخدام ميزه سجل التدقيق. لاسترداد الرسائل المحذوفة في Outlook علي الويب ، راجع [استرداد العناصر المحذوفة في Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
