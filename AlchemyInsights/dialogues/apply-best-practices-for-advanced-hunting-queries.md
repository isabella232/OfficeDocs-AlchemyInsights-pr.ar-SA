---
title: تطبيق أفضل الممارسات للاستعلامات المتقدمة حول البحث
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
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692627"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>تطبيق أفضل الممارسات للاستعلامات المتقدمة حول البحث

للحصول على النتائج بشكل أسرع وتجنب المهات أثناء تشغيل الاستعلامات المعقدة، قم بتطبيق أفضل الممارسات التالية:

- عند تجربة استعلامات جديدة، استخدم دائما حد، لتجنب الحصول على مجموعات نتائج كبيرة جدا. أيضا، `count` يتم استخدامها لإعداد تقييم أولي لحجم مجموعة النتائج.
- استخدم عوامل تصفية الوقت أولا. وبشكل مثالي، حصر الاستعلامات بسبعة أيام.
- في بداية الاستعلام، بعد عامل تصفية الوقت مباشرة، أضف عوامل التصفية المتوقعة لإزالة معظم البيانات.
- عند البحث عن الرموز المميزة الكاملة، استخدم `has` عامل التشغيل بدلا من `contains` .
- يمكنك تشغيل عملية بحث على عمود معين بدلا من تشغيلها عبر كل الأعمدة.
- عند ضم الجداول، حدد الجدول الذي به صفوف أقل أولا.
- `project` الأعمدة الضرورية فقط من الجداول التي قمت بضمها.

لمعرفة المزيد، راجع أفضل ممارسات استعلام [البحث المتقدم.](https://go.microsoft.com/fwlink/?linkid=2144812)
