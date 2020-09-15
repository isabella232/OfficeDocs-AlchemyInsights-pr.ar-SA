---
title: تبديل الموقع الجذر الكلاسيكي باستخدام موقع حديث
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
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691166"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>تبديل الموقع الجذر الكلاسيكي باستخدام موقع حديث

إذا تم اعداد البيئة الخاصة بك قبل 2019 ابريل ، يمكنك تغيير الموقع الجذر إلى موقع حديث باستخدام Microsoft PowerShell:

- إذا كان لديك موقع مختلف تريد استخدامه كموقع جذر ، يمكنك استبدال [(تبديل) الموقع الجذر](https://docs.microsoft.com/sharepoint/modern-root-site) به. 
    - استخدم [Invoke-سبوسيتيسواب](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لتبديل موقع الموقع مع موقع آخر اثناء أرشفه الموقع الأصلي. متوفر لكل من موقع الفريق (غير متصل بمجموعه) وموقع الاتصال. 

- سيتم تقديم قدرات اضافيه قريبا مما سيسمح لك بالاستمرار في استخدام المحتوي علي الموقع ، ولكن يمكنك تحويل الموقع الموجود إلى موقع اتصال. 
>[!Important]
>سيتم عكس هذه الإمكانيات تدريجيا. تابع التحقق من مركز الرسائل للحصول علي تحديثات. 

## <a name="known-issues-with-swapping-sites"></a>المشاكل المعروفة في مواقع التبادل

- قد يرجع الموقع الهدف الخطا "لم يتم العثور عليه" (HTTP 404) لفتره قصيرة من الوقت.
- سيحتاج المحتوي إلى ريكراوليد لتحديث فهرس البحث. لا توجد خطوه يدوية مطلوبه-سيتم القيام بذلك تلقائيا.
- يجب تصحيح اي شيء يعتمد علي ارتباطات "static" (مثل مزامنة الملفات وملفات OneNote) يدويا.
- إذا كان الموقع المصدر عبارة عن موقع اخبار تنظيميه ، فقم بتحديث عنوان URL.احصل علي قائمه بكل مواقع الاخبار التنظيمية.
- قد يلزم التحقق من صحة مواقع Project Server لضمان انها لا تزال مقترنة بشكل صحيح.
