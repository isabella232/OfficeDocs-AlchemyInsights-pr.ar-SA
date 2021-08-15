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
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981100"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>خطأ: القواعد على هذا الكمبيوتر غير متطابقة

لرؤية الحالة المحدثة لهذه المشكلة المعروفة، راجع القواعد على هذا الكمبيوتر لا تتطابق [مع القواعد على Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

لقد Outlook فريق العمل تصحيحا في البنية 12928.10000. الإصلاح موجود بالفعل في Insider Fast وسيذهب إلى القناة الشهرية في أواخر يونيو 2020. بمجرد الحصول على البنية الثابتة، قد تحصل على المطالبة "ما هي القواعد التي تريد الاحتفاظ بها" مرة واحدة أخيرة. اختر الخادم عند مطالبتك بذلك، ثم ارجع إلى Outlook ثم اعاد تمكين أي قواعد تم تعطيلها.

حتى يتوفر الإصلاح، الرجاء استخدام الحل البديل التالي:

**الحل البديل**: في التقارير الأخيرة، حدثت المشكلة لهؤلاء الذين لم ينشئوا سوى قواعد العميل في Outlook سطح المكتب. إذا استمرت المشكلة، فنظر في حذف القواعد ثم قم بإنشاء القواعد وتحريرها فقط في OWA (Outlook Web App) حتى يتم حل المشكلة.

إذا لم تتمكن من حذف القواعد يدويا، يمكنك تشغيل أمر Outlook عند بدء Outlook بتشغيل Outlook.exe /cleanrules. سيحذف هذا كلا من قواعد العميل وخادم. سيتم حذف كل القواعد لكل الحسابات في ملف Outlook التعريف. تم توثيق هذا الأمر بشكل أكبر في مقالة تبديل سطر الأوامر.

