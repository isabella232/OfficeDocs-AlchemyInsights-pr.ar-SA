---
title: قاعدة DLP ل رقم بطاقة الائتمان لا تعمل
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
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005077"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>مشاكل DLP مع أرقام بطاقات الائتمان

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

**مشاكل DLP مع أرقام بطاقات الائتمان**

هل تواجه مشاكل في منع فقدان البيانات **(DLP)** لا تعمل على محتوى يحتوي على رقم بطاقة ائتمان عند استخدام نوع معلومات حساسة ل DLP في O365؟  إذا كان الأمر كذلك، فتأكد من أن المحتوى يحتوي على المعلومات المطلوبة لتحريك نهج DLP عند تقييمه. على سبيل المثال، بالنسبة إلى نهج بطاقة الائتمان الذي تم تكوينه بمستوى ثقة بنسبة 85٪، يتم تقييم ما يلي ويجب اكتشافه حتى يتم تشغيل القاعدة: 
  
- **[التنسيق:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 رقما يمكن تنسيقها أو عدم تنسيقها (ddddddd) ويجب أن تجتاز اختبار Luhn.

- **[النمط:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** النمط شديد التعقيد والقوة الذي يكشف عن البطاقات من جميع العلامات التجارية الرئيسية في جميع أنحاء العالم، بما في ذلك بطاقات Visa و MasterCard وD discover Card و JCB و American Express وبطاقات الهدايا وبطاقات العشاء.

- **[الاختبارات:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** نعم، فحص لوهين

- **[التعريف:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** إن نهج DLP واثق بنسبة 85٪ من أنه تم الكشف عن هذا النوع من المعلومات الحساسة إذا، ضمن تقارب 300 حرف:

  - تعثر الدالة Func_credit_card المحتوى الذي يتطابق مع النمط.

  - يكون أحد ما يلي صحيحا:

  - تم العثور على كلمة أساسية Keyword_cc_verification كلمة أساسية.

  - تم العثور على كلمة أساسية Keyword_cc_name كلمة أساسية

  - تعثر Func_expiration_date الدالة على تاريخ بتنسيق التاريخ المناسب.

  - تمريرات الاختبارات

    على سبيل المثال، قد يؤدي النموذج التالي إلى تشغيل نهج رقم بطاقة ائتمان DLP:

  - Visa: 4485 3647 3952 7352
  
  - تنتهي الصلاحية: 2/2/2009

للحصول على مزيد من المعلومات  حول ما هو مطلوب للكشف عن رقم بطاقة الائتمان للمحتوى الخاص بك، راجع المقطع التالي في هذه المقالة: ما تبحث عنه أنواع المعلومات الحساسة [لبطاقة الائتمان#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
باستخدام نوع مختلف من المعلومات الحساسة المضمنة، راجع المقالة التالية للحصول على معلومات حول ما هو مطلوب للأنواع الأخرى: ما تبحث عنه أنواع المعلومات [الحساسة](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  