---
title: مبادله موقع الجذر الكلاسيكي الخاص بك مع موقع حديث
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36749247"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>مبادله موقع الجذر الكلاسيكي الخاص بك مع موقع حديث

إذا تم اعداد البيئة الخاصة بك قبل 2019 ابريل ، يمكنك تغيير موقع الجذر إلى موقع حديث باستخدام Microsoft PowerShell:

- إذا كان لديك موقع آخر تريد استخدامه كموقع الجذر الخاص بك ، يمكنك استبدال [(مبادله) موقع الجذر](https://docs.microsoft.com/sharepoint/modern-root-site) معها. 
    - استخدام [استدعاء-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لمبادله موقع موقع مع موقع آخر اثناء أرشفه الموقع الأصلي. متوفر لكل من موقع الفريق (غير متصل بمجموعه) وموقع الاتصالات. 

- سيتم تقديم قدرات اضافيه قريبا من شانها ان تسمح لك للحفاظ علي استخدام المحتوي علي الموقع ، ولكن تحويل الموقع الحالي إلى موقع الاتصالات. 
>[!Important]
>سيتم نشر هذه القدرات تدريجيا. متابعه التحقق من مركز الرسائل 365 Office للحصول علي التحديثات. 

## <a name="known-issues-with-swapping-sites"></a>المشكلات المعروفة مع تبادل المواقع

- قد يرجع الموقع الهدف خطا "لم يتم العثور علي" (HTTP 404) لفتره قصيرة من الوقت.
- سيحتاج المحتوي إلى أعاده التصنيف لتحديث فهرس البحث. لا توجد خطوه يدوية مطلوبه-سيتم ذلك تلقائيا.
- اي شيء يعتمد علي الارتباطات "الثابتة" (مثل مزامنة الملفات وملفات OneNote) سوف تحتاج إلى تصحيح يدويا.
- إذا كان موقع المصدر موقعا إخباريا تنظيميا ، فقم بتحديث عنوان URL.الحصول علي قائمه بجميع المواقع الاخباريه التنظيمية.
- قد تحتاج مواقع خادم Project إلى التحقق من صحتها للتاكد من انها لا تزال مقترنة بشكل صحيح.





