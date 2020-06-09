---
title: 'خطأ: القواعد على هذا الكمبيوتر لا تتطابق'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617948"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>خطأ: القواعد على هذا الكمبيوتر لا تتطابق

لمشاهدة الحالة المحدثة لهذه المشكلة المعروفة، راجع [القواعد على هذا الكمبيوتر لا تتطابق مع القواعد على Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

قام فريق Outlook بتنفيذ إصلاح في بناء 12928.10000. الإصلاح هو بالفعل في منالداخل السريع وسوف تذهب إلى القناة الشهرية في أواخر يونيو 2020. وبمجرد الانتهاء من بناء ثابت قد تحصل على موجه "القواعد التي تريد الاحتفاظ بها" مرة أخيرة. اختر الخادم عند المطالبة ثم العودة في Outlook وإعادة تمكين أي قواعد تم تعطيلها.

حتى يتوفر الإصلاح الرجاء استخدام الحل التالي:

**الحل البديل:** في التقارير الأخيرة، حدثت المشكلة لتلك التي أنشأت قواعد العميل فقط في سطح مكتب Outlook. إذا كنت لا تزال تواجه المشكلة، خذ بعين الاعتبار حذف القواعد ثم إنشاء القواعد وتحريرها فقط في OWA (Outlook Web App) حتى يتم حل المشكلة.

إذا لم تتمكن من حذف القواعد يدوياً يمكنك تشغيل أمر Outlook عند بدء تشغيل Outlook عن طريق تشغيل Outlook.exe /cleanrules. سيؤدي ذلك إلى حذف كل من قواعد العميل والملقم. فإنه سيتم حذف كافة القواعد لكافة الحسابات في ملف تعريف Outlook. يتم توثيق هذا الأمر في مقالة مفاتيح سطر الأوامر.