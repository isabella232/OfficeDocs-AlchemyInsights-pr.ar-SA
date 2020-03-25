---
title: قاعدة DLP لرقم بطاقة الائتمان لا يعمل
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932430"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>مشكلات DLP مع أرقام بطاقات الائتمان

**هام:** يعمل العديد من عملاء SharePoint Online و OneDrive على تشغيل تطبيقات مهمة للأعمال مقابل الخدمة التي تعمل في الخلفية. وتشمل هذه ترحيل المحتوى، منع فقدان البيانات (DLP)، وحلول النسخ الاحتياطي. خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية وموثوقة للمستخدمين الذين يعتمدون على الخدمة أكثر من أي وقت مضى في سيناريوهات العمل عن بعد.

ولدعم هذا الهدف، قمنا بتنفيذ قيود خنق أكثر صرامة على تطبيقات الخلفية (الترحيل وDLP وحلول النسخ الاحتياطي) خلال ساعات النهار في أيام الأسبوع. يجب أن تتوقع أن تحقق هذه التطبيقات إنتاجية محدودة جدًا خلال هذه الأوقات. ومع ذلك ، خلال ساعات المساء وعطلة نهاية الأسبوع للمنطقة ، ستكون الخدمة جاهزة لمعالجة حجم أكبر بكثير من الطلبات من تطبيقات الخلفية.

**مشكلات DLP مع أرقام بطاقات الائتمان**

هل تواجه مشاكل مع **منع فقدان البيانات (DLP)** لا تعمل للمحتوى الذي يحتوي على **رقم بطاقة الائتمان** عند استخدام نوع معلومات حساسة DLP في O365؟ إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لتشغيل نهج DLP عند تقييمه. على سبيل المثال، بالنسبة **لسياسة بطاقة الائتمان** التي تم تكوينها بمستوى ثقة 85%، يتم تقييم ما يلي ويجب الكشف عنها حتى تقوم القاعدة بتشغيلها:
  
- **[التنسيق:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 رقمًا يمكن تنسيقها أو عدم تنسيقها (ddddddddddddd) ويجب أن تجتاز اختبار Luhn.

- **[نمط:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** نمط معقد وقوي للغاية يكشف البطاقات من جميع العلامات التجارية الكبرى في جميع أنحاء العالم ، بما في ذلك فيزا ، ماستركارد ، بطاقة ديسكفري ، JCB ، أمريكان إكسبريس ، بطاقات الهدايا ، وبطاقات العشاء.

- **[المجموع الاختياري:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** نعم، مجموع الاختيار لوهن

- **[التعريف:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** سياسة DLP واثقة بنسبة 85٪ من أنها اكتشفت هذا النوع من المعلومات الحساسة إذا، على مقربة من 300 حرف:

  - Func_credit_card الدالة البحث عن المحتوى الذي يطابق النمط.

  - أحد ما يلي هو الصحيح:

  - تم العثور على كلمة رئيسية من Keyword_cc_verification.

  - تم العثور على كلمة رئيسية من Keyword_cc_name

  - Func_expiration_date الدالة البحث عن تاريخ بتنسيق التاريخ الصحيح.

  - يمر المجموع الاختياري

    على سبيل المثال، سيتم تشغيل العينة التالية لسياسة رقم بطاقة الائتمان DLP:

  - التأشيرة: 4485 3647 3952 7352
  
  - تنتهي صلاحيتها: 2/2009

لمزيد من المعلومات حول ما هو مطلوب للكشف عن **رقم بطاقة الائتمان** للمحتوى الخاص بك، راجع القسم التالي في هذه المقالة: ما أنواع المعلومات [الحساسة البحث عن بطاقة الائتمان#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
باستخدام نوع معلومات حساسة مضمن ة مختلفة، راجع المقالة التالية للحصول على معلومات حول ما هو مطلوب للأنواع الأخرى: [ما تبحث عنه أنواع المعلومات الحساسة](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  