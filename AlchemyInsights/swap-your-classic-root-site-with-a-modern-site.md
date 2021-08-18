---
title: تبديل موقعك الجذر الكلاسيكي مع موقع حديث
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316127"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>تبديل موقعك الجذر الكلاسيكي مع موقع حديث

إذا تم إعداد بيئتك قبل أبريل 2019، يمكنك تغيير موقعك الجذر إلى موقع حديث باستخدام Microsoft PowerShell:

- إذا كان لديك موقع آخر تريد استخدامه كم موقع الجذر، يمكنك استبدال [(تبديل)](https://docs.microsoft.com/sharepoint/modern-root-site) الموقع الجذر به. 
    - استخدم [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لتبديل موقع موقع بموقع آخر أثناء أرشفة الموقع الأصلي. يتوفر لكل من موقع الفريق (غير متصل بمجموعة) و"موقع الاتصالات". 

- سيتم توفير إمكانات إضافية قريبا تتيح لك الاستمرار في استخدام المحتوى على الموقع، ولكن تحويل الموقع الموجود إلى موقع اتصال. 

**هام:** سيتم طرح هذه الإمكانات تدريجيا. تابع التحقق من مركز الرسائل للحصول على التحديثات. 

## <a name="known-issues-with-swapping-sites"></a>المشاكل المعروفة في تبديل المواقع

- قد يرجع الموقع الهدف الخطأ "لم يتم العثور عليه" (HTTP 404) لفترة زمنية قصيرة.
- يجب إعادة فهرسة المحتوى لتحديث فهرس البحث. لا توجد خطوة يدوية مطلوبة - سيتم إجراء ذلك تلقائيا.
- يجب تصحيح أي شيء يعتمد على الارتباطات "الثابتة" (مثل OneNote الملفات ومزامنة الملفات) يدويا.
- إذا كان الموقع المصدر هو موقع أخبار المؤسسة، فحدث عنوان URL. احصل على قائمة بكل مواقع أخبار المؤسسة.
- Project قد تحتاج مواقع الخوادم إلى التحقق من صحتها للتأكد من أنها لا تزال مقترنة بشكل صحيح.
