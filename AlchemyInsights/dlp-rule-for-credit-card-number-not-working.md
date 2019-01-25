---
title: رقم بطاقة الائتمان لا تعمل قاعدة DLP
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: a56f32b54e6cb32fa044d26d08868bac8c368de5
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29456413"
---
هل تواجه مشاكل في **منع فقدان البيانات (DLP)** لا يعمل للمحتوى الذي يحتوي على **رقم بطاقة الائتمان** عند استخدام نوع معلومات حساسة DLP في O365؟ إذا كان الأمر كذلك، تأكد من المحتوى الخاص بك يحتوي على المعلومات المطلوبة لتشغيل نهج DLP عندما يتم تقييمه. على سبيل المثال، **بطاقة الائتمان نهج** تكوين بمستوى ثقة 85 في المائة، التالية يتم تقييمها ويجب الكشف عن لتشغيل القاعدة: 
  
- **[تنسيق:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** رقم 16 التي يمكن تنسيقها أو غير منسق (ددددددددددددددد) ويجب أن يجتاز اختبار ليون. 
    
- **[نموذج:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** نمط معقد للغاية وفعالية الكشف عن بطاقات من جميع العلامات التجارية الكبرى في العالم، بما في ذلك التأشيرات Mastercard، اكتشاف بطاقة، JCB، أمريكان إكسبريس، بطاقات الهدايا وبطاقات العشاء. 
    
- **[المجموع الاختباري:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** نعم، كان المجموع الاختباري ليون 
    
- **[تعريف:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** هو نهج DLP 85% واثقاً من الكشف عن هذا النوع من المعلومات الهامة إذا مسافة 300 حرف: 
    
  - دالة Func_credit_card البحث عن المحتوى الذي يطابق النموذج.
    
  - أي مما يلي صحيحاً: 
    
  - تم العثور على كلمة أساسية من Keyword_cc_verification.
    
  - تم العثور على كلمة أساسية من Keyword_cc_name
    
  - دالة Func_expiration_date عن تاريخ في تنسيق التاريخ الصحيح.
    
  - مسارات المجموع الاختباري
    
    على سبيل المثال، النموذج التالي سيثير "نهج DLP رقم بطاقة الائتمان":
    
  - تأشيرة المرور: 7352 3952 3647 4485 
    
  - انتهاء الصلاحية: 2/2009
    
لمزيد من المعلومات حول ما هو مطلوب **رقم بطاقة الائتمان** ليتم اكتشافها للمحتوى، راجع المقطع التالي في هذا المقال: [ما الحساسة معلومات الأنواع ابحث عن بطاقة الائتمان #](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
استخدام نوع معلومات حساسة مضمنة مختلفة، راجع المقالة التالية للحصول على المعلومات على ما هو مطلوب للأنواع الأخرى: [البحث عن "ما الحساسة معلومات الأنواع"](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

