---
title: 'خطأ: القواعد على هذا الكمبيوتر غير متطابقة'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782939"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>خطأ: القواعد على هذا الكمبيوتر غير متطابقة

لرؤية الحالة المحدثة لهذه المشكلة المعروفة، راجع القواعد على هذا الكمبيوتر لا تتطابق [مع القواعد في Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

نفذ فريق Outlook تصحيحا في البنية 12928.10000. الإصلاح موجود بالفعل في Insider Fast وسيذهب إلى القناة الشهرية في أواخر يونيو 2020. بمجرد الحصول على البنية الثابتة، قد تحصل على المطالبة "ما هي القواعد التي تريد الاحتفاظ بها" مرة واحدة أخيرة. اختر الخادم عند مطالبتك بذلك، ثم ارجع إلى Outlook ثم اعاد تمكين أي قواعد تم تعطيلها.

حتى يتوفر الإصلاح، الرجاء استخدام الحل البديل التالي:

**الحل البديل**: في التقارير الأخيرة، حدثت المشكلة لهؤلاء الذين أنشأوا قواعد العميل فقط في Outlook لسطح المكتب. إذا استمرت المشكلة، فنظر في حذف القواعد ثم قم بإنشاء القواعد وتحريرها فقط في OWA (Outlook Web App) حتى يتم حل المشكلة.

إذا لم تتمكن من حذف القواعد يدويا، يمكنك تشغيل أمر Outlook عند بدء تشغيل Outlook عن طريق تشغيل Outlook.exe /cleanrules. سيحذف هذا كلا من قواعد العميل وخادم. سيتم حذف كل القواعد لكل الحسابات في ملف تعريف Outlook. تم توثيق هذا الأمر بشكل أكبر في مقالة تبديل سطر الأوامر.

