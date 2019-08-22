---
title: تبديل الموقع الجذر التقليدية مع موقع الحديثة
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501066"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>تبديل الموقع الجذر التقليدية مع موقع الحديثة

إذا تم إعداد البيئة الخاصة بك قبل نيسان/أبريل عام 2019، يمكنك تغيير الموقع الجذر الخاص بك إلى موقع حديثة باستخدام Microsoft PowerShell:

- إذا كان لديك موقع آخر تريد استخدامه كالموقع الجذر الخاص بك، يمكنك استبدال (ترحيل) الجذر الموقع معها. 
    - استخدام [استدعاء سبوسيتيسواب](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لتبديل موضع موقع بموقع آخر أثناء الأرشفة الموقع الأصلي. يتوفر لكل موقع الفريق (غير متصل بمجموعة) وموقع الاتصال. 

- تم توفير قدرات إضافية قريبا التي تسمح لك للاحتفاظ باستخدام المحتوى على الموقع، ولكن تحويل موقع موجود إلى موقع اتصال. 
>[!Important]
>هذه القدرات سيبدأ تدريجيا. متابعة للتحقق من مركز الرسائل Office 365 للتحديثات. 

## <a name="known-issues-with-swapping-sites"></a>المشكلات المعروفة المتعلقة بتبادل المواقع

- موقع الهدف قد بإرجاع خطأ (HTTP 404) "لم يتم العثور على" لفترة قصيرة من الوقت.
- أن محتوى تتبع الارتباطات من جديد لتحديث فهرس البحث. خطوة ليست اليدوية المطلوبة-هذا يتم إنجازه تلقائياً.
- أي شيء يعتمد على روابط "ثابتة" (مثل ملفات OneNote ومزامنة الملفات) ستحتاج إلى تصحيحه يدوياً.
- إذا كان موقع المصدر موقع أخبار المؤسسة، تحديث عنوان URL.الحصول على قائمة بكافة مواقع أخبار المؤسسة.
- قد تحتاج مواقع المشروع على الخادم التحقق من صحة للتأكد من أنها لا يزال مرتبطاً بشكل صحيح.





