---
title: مخزون البرامج مفقود أو غير دقيق
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676049"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>مخزون البرامج مفقود أو غير دقيق

إن مخزون البرامج في إدارة المخاطر والثغرات الأمنية (TVM) هو قائمة البرامج المعروفة في مؤسستك باستخدام تعدادات النظام الأساسي الشائع (CPE) الرسمية.

لا يتم نشر نقاط الضعف في منتجات البرامج التي لا تملك CPE رسمية. يتضمن المخزون أيضا تفاصيل مثل اسم المورد وعدد نقاط الضعف والتهديدات وعدد الأجهزة التي يتم عرضها.

تنعكس تغييرات البرامج على الأجهزة عادة في مداخل الأمان في غضون ساعتين. ومع ذلك، قد يستغرق الأمر في بعض الأحيان وقتا أطول. لا توجد حاليا أي طريقة فرض المزامنة؛ هذا تقييم مستمر مستمر.

إذا قمت بتغيير البرنامج ولم يظهر التغيير بدقة في TVM بعد مرور 5 ساعات، فاتبع الخطوات التالية:

1. تحقق من قسم دليل البرنامج لفهم كيفية اكتشاف البرنامج.
1. تأكد من دعم البرنامج. قد يكون البرنامج مرئيا فقط على مستوى الجهاز حتى لو لم يكن مدعوما حاليا من قبل إدارة المخاطر والثغرات الأمنية. ومع ذلك، لا تتوفر سوى بيانات محدودة.
1. للحصول على خطوات الإبلاغ عن عدم الدقة من المدخل، راجع [الإبلاغ عن عدم الدقة](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).
   
    **ملاحظة:** الإبلاغ عن عدم دقة من مدخل MDE هو قناة ذات طريقة واحدة إلى الهندسة. إذا كانت المشكلة عاجلة، فافتح تذكرة دعم.

لمزيد من المعلومات، راجع [مخزون البرامج - إدارة المخاطر والثغرات الأمنية](/microsoft-365/security/defender-endpoint/tvm-software-inventory).