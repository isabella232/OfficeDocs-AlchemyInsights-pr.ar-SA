---
title: قاعده DLP لرقم بطاقة الائتمان لا يعمل
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679428"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>مشاكل DLP مع أرقام بطاقات الائتمان

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

**مشاكل DLP مع أرقام بطاقات الائتمان**

هل تواجه مشاكل متعلقة **بمنع فقدان البيانات (DLP)** لا تعمل علي المحتوي الذي يحتوي علي **رقم بطاقة ائتمان** عند استخدام نوع معلومات الحساسية ل DLP في O365 ؟ إذا كان الأمر كذلك ، فتاكد من ان المحتوي يحتوي علي المعلومات المطلوبة لتشغيل نهج DLP عند تقييمه. علي سبيل المثال ، بالنسبة **لسياسة بطاقة الائتمان** التي تم تكوينها باستخدام مستوي الثقة في 85% ، يتم تقييم التالية ويجب الكشف عنها ليتم تشغيل القاعدة:
  
- **[تنسيق:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 خانه رقميه يمكن تنسيقها أو تهيئتها (ددددددددددددددد) ويجب ان تمرر اختبار لوهن.

- **[النمط:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** نمط معقد جدا وقوي يقوم بالكشف عن البطاقات من كل المنتجات الرئيسية في انحاء العالم ، بما في ذلك التاشيره والMasterCard والكشف عن البطاقات والJCB فالامريكيه وبطاقات الهدايا وبطاقات دينير.

- **[المجموع الاختباري:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** نعم ، المجموع الاختباري للوهن

- **[تعريف:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** نهج DLP هو 85% تثق بأنه قد تم اكتشاف هذا النوع من المعلومات الهامه في حال وجوده في غضون أكثر من 300 حرفا:

  - تعثر الدالة Func_credit_card علي المحتوي الذي يتطابق مع النمط.

  - يعد أحد الخيارات التالية صحيحا:

  - تم العثور علي كلمه أساسيه من Keyword_cc_verification.

  - تم العثور علي كلمه أساسيه من Keyword_cc_name

  - تعثر الدالة Func_expiration_date علي تاريخ بتنسيق التاريخ الصحيح.

  - يمرر المجموع الاختباري

    علي سبيل المثال ، سيتم تشغيل النموذج التالي لنهج رقم بطاقة ائتمان DLP:

  - التاشيره: 4485 3647 3952 7352
  
  - تنتهي الصلاحية: 2/2009

للحصول علي مزيد من المعلومات حول ما هو مطلوب لاكتشاف **رقم بطاقة الائتمان** للمحتوي ، راجع القسم التالي في هذه المقالة: [ما الذي تبحث عنه أنواع المعلومات الحساسة عن بطاقة الائتمان #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
باستخدام نوع آخر من المعلومات الحساسة المضمنة ، راجع المقالة التالية للحصول علي معلومات حول ما هو مطلوب للأنواع الأخرى: [ما الذي تبحث عنه أنواع المعلومات الهامه](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  