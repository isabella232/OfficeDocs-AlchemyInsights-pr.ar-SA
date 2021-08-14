---
title: تطبيق أفضل الممارسات لاستعلامات الصيد المتقدمة
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930120"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>تطبيق أفضل الممارسات لاستعلامات الصيد المتقدمة

للحصول على النتائج بشكل أسرع وتجنب المهات أثناء تشغيل الاستعلامات المعقدة، طبق أفضل الممارسات التالية:

- عند تجربة استعلامات جديدة، استخدم دائما حد لتجنب الحصول على مجموعات نتائج كبيرة جدا. أيضا، استخدم هذا التقييم لتقييم أولي لحجم `count` مجموعة النتائج.
- استخدم عوامل تصفية الوقت أولا. وبشكل مثالي، حصر الاستعلامات بسبعة أيام.
- في بداية استعلام، بعد عامل تصفية الوقت مباشرة، أضف عوامل التصفية المتوقعة لإزالة معظم البيانات.
- عند البحث عن الرموز المميزة الكاملة، استخدم `has` عامل التشغيل بدلا من `contains` .
- يمكنك تشغيل عملية بحث على عمود معين بدلا من تشغيلها عبر كل الأعمدة.
- عند الانضمام إلى الجداول، حدد الجدول الذي به صفوف أقل أولا.
- `project` الأعمدة الضرورية فقط من الجداول التي قمت بضمها.

لمعرفة المزيد، راجع [أفضل ممارسات استعلام البحث المتقدم](https://go.microsoft.com/fwlink/?linkid=2144812).
