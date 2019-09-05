---
title: مبادلة موقع الجذر الكلاسيكي الخاص بك مع موقع حديث
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
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36749247"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>مبادلة موقع الجذر الكلاسيكي الخاص بك مع موقع حديث

إذا تم إعداد البيئة الخاصة بك قبل أبريل عام 2019، يمكنك تغيير الموقع الجذر إلى موقع حديث باستخدام Microsoft PowerShell:

- إذا كان لديك موقع مختلف تريد استخدامه كموقع جذر، يمكنك استبدال [(مبادلة) الموقع الجذر](https://docs.microsoft.com/sharepoint/modern-root-site) معه. 
    - استخدم [استدعاء SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لمبادلة موقع موقع مع موقع آخر أثناء أرشفة الموقع الأصلي. متوفر لكل من موقع الفريق (غير متصل بمجموعة) وموقع الاتصال. 

- سيتم تقديم قدرات إضافية قريباً تسمح لك بالاستمرار في استخدام المحتوى على الموقع، ولكن تحويل الموقع الحالي إلى موقع اتصال. 
>[!Important]
>وسيتم نشر هذه القدرات تدريجيا. تابع التحقق من معلومات مركز رسائل Office 365 عن التحديثات. 

## <a name="known-issues-with-swapping-sites"></a>المشكلات المعروفة مع مواقع المبادلة

- قد يرجع الموقع الهدف خطأ "لم يتم العثور عليها" (HTTP 404) لفترة قصيرة من الوقت.
- يجب إعادة تتبع ارتباطات المحتوى لتحديث فهرس البحث. لا توجد خطوة يدوية مطلوبة - سيتم ذلك تلقائيا.
- يجب تصحيح أي شيء يعتمد على الارتباطات "الثابتة" (مثل مزامنة الملف وملفات OneNote) يدويًا.
- إذا كان الموقع المصدر موقع أخبار تنظيمية، فحدّث عنوان URL.الحصول على قائمة بجميع مواقع الأخبار التنظيمية.
- قد تحتاج مواقع خادم Project إلى التحقق من صحة للتأكد من أنها لا تزال مقترنة بشكل صحيح.





