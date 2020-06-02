---
title: تحديد أحداث حذف الرسائل في سجلات التدقيق
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508975"
---
# <a name="audit-logs-for-deleted-email-messages"></a>سجلات التدقيق لرسائل البريد الإلكتروني المحذوفة

بدءًا من يناير 2019، تقوم Microsoft بتشغيل تسجيل تدقيق علبة البريد بشكل افتراضي. وإلا، لمراجعة أحداث حذف الرسائل لمستخدم معين، تحتاج إلى تمكين إجراءات الحذف للتدقيق يدويًا. إذا تم بالفعل تمكين تسجيل تدقيق علبة البريد لمؤسستك أو للمستخدم المحدد، فاتبع الخطوات التالية.

1. تسجيل الدخول إلى [مركز التوافق & الأمان Microsoft 365](https://protection.office.com/)

2. انقر فوق **البحث والتحقيق** وحدد بحث **سجل التدقيق**.

3. حدد نطاق التاريخ في **حقول تاريخ البدء** وتاريخ **الانتهاء.** حدد اسم المستخدم للمستخدم الذي تريد التحقيق (المستخدم الذي حذف العناصر). في حقل **الأنشطة،** حدد **الرسائل المحذوفة من مجلد العناصر المحذوفة** **والرسائل التي تم نقلها إلى مجلد العناصر المحذوفة**.

4. انقر فوق **البحث**.

في النتائج، حدد سجل تدقيق. في التفاصيل المنبثقة، انقر فوق **مزيد من المعلومات**. يتم عرض معلومات إضافية حول العنصر المحذوف (على سبيل المثال، سطر الموضوع وموقع العنصر عند حذفه) في حقل **العناصر المتأثرة.** ستظهر خاصية **ClientInfoString** إذا حدث الحذف في Outlook أو Outlook على الويب (المعروف سابقًا باسم Outlook Web App) أو أي جهاز آخر.

لمزيد من المعلومات، راجع [تحديد من قام بإعداد إعادة توجيه البريد الإلكتروني لعلبة بريد](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**ملاحظة:** لا يمكنك استرداد العناصر المحذوفة باستخدام ميزة سجل التدقيق. لاسترداد الرسائل المحذوفة في Outlook على الويب، راجع [استرداد العناصر المحذوفة في Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
