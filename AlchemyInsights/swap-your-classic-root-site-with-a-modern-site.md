---
title: مبادلة موقع الجذر الكلاسيكي الخاص بك مع موقع حديث
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741531"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>مبادلة موقع الجذر الكلاسيكي الخاص بك مع موقع حديث

إذا تم إعداد البيئة الخاصة بك قبل أبريل 2019، يمكنك تغيير موقع الجذر الخاص بك إلى موقع حديث باستخدام Microsoft PowerShell:

- إذا كان لديك موقع مختلف تريد استخدامه كموقع الجذر الخاص بك، يمكنك استبدال [(مبادلة) موقع الجذر](https://docs.microsoft.com/sharepoint/modern-root-site) معه. 
    - استخدم [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لتبديل موقع موقع مع موقع آخر أثناء أرشفة الموقع الأصلي. متوفر لكل من موقع الفريق (غير متصل بمجموعة) وموقع الاتصال. 

- سيتم تقديم قدرات إضافية قريبًا تسمح لك بمواصلة استخدام المحتوى على الموقع ، ولكن تحويل الموقع الحالي إلى موقع اتصال. 
>[!Important]
>وسيتم نشر هذه القدرات تدريجيا. متابعة التحقق من مركز الرسائل للحصول على التحديثات. 

## <a name="known-issues-with-swapping-sites"></a>المشكلات المعروفة مع مواقع المبادلة

- قد يرجع الموقع المستهدف خطأ "لم يتم العثور عليه" (HTTP 404) لفترة قصيرة من الزمن.
- يجب إعادة كتابة المحتوى لتحديث فهرس البحث. لا توجد خطوة يدوية مطلوبة - سيتم ذلك تلقائيًا.
- أي شيء يعتمد على الارتباطات "الثابتة" (مثل مزامنة الملفات وملفات OneNote) سيحتاج إلى تصحيح يدويًا.
- إذا كان موقع المصدر موقعًا إخباريًا تنظيميًا، فقم بتحديث عنوان URL.احصل على قائمة بجميع المواقع الإخبارية التنظيمية.
- قد تحتاج مواقع Project Server إلى التحقق من صحتها للتأكد من أنها لا تزال مقترنة بشكل صحيح.
