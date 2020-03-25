---
title: قاعدة DLP لـ SSN لا تعمل
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932502"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP القضايا مع أرقام الضمان الاجتماعي

**هام:** يعمل العديد من عملاء SharePoint Online و OneDrive على تشغيل تطبيقات مهمة للأعمال مقابل الخدمة التي تعمل في الخلفية. وتشمل هذه ترحيل المحتوى، منع فقدان البيانات (DLP)، وحلول النسخ الاحتياطي. خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية وموثوقة للمستخدمين الذين يعتمدون على الخدمة أكثر من أي وقت مضى في سيناريوهات العمل عن بعد.

ولدعم هذا الهدف، قمنا بتنفيذ قيود خنق أكثر صرامة على تطبيقات الخلفية (الترحيل وDLP وحلول النسخ الاحتياطي) خلال ساعات النهار في أيام الأسبوع. يجب أن تتوقع أن تحقق هذه التطبيقات إنتاجية محدودة جدًا خلال هذه الأوقات. ومع ذلك ، خلال ساعات المساء وعطلة نهاية الأسبوع للمنطقة ، ستكون الخدمة جاهزة لمعالجة حجم أكبر بكثير من الطلبات من تطبيقات الخلفية.

**مشكلات DLP مع SSNs**

هل تواجه مشاكل مع **منع فقدان البيانات (DLP)** لا تعمل للمحتوى الذي يحتوي على **رقم الضمان الاجتماعي (SSN)** عند استخدام نوع معلومات حساسة في Office 365؟ إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لما تبحث عنه سياسة DLP. 
  
على سبيل المثال، بالنسبة لسياسة SSN التي تم تكوينها بمستوى ثقة 85%، يتم تقييم ما يلي ويجب الكشف عنها حتى تقوم القاعدة بتشغيلها:
  
- **[التنسيق:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 أرقام، والتي قد تكون في نمط منسق أو غير منسق

- **[نمط:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** أربع وظائف تبحث عن SSNs في أربعة أنماط مختلفة:

  - Func_ssn يجد SSNs مع التنسيق القوي قبل عام 2011 التي يتم تنسيقها مع شرطات أو مسافات (ddd-ddddd or ddd ddddddddddddddddddddddddddddddddddddddddd

  - Func_unformatted_ssn يجد SSNs مع التنسيق قوية قبل 2011 التي لم يتم تنسيقها كتسعة أرقام متتالية (ddddddddd)

  - Func_randomized_formatted_ssn يجد SSNs ما بعد 2011 التي تم تنسيقها مع شرطات أو مسافات (ddd-ddddd or ddd dddddddddddd)

  - Func_randomized_unformatted_ssn يجد SSNs ما بعد 2011 التي لم يتم تنسيقها كتسعة أرقام متتالية (ddddddddd)

- **[المجموع الاختياري:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** لا، لا يوجد المجموع الاختياري

- **[التعريف:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** سياسة DLP واثقة بنسبة 85٪ من أنها اكتشفت هذا النوع من المعلومات الحساسة إذا، على مقربة من 300 حرف:

  - Func_ssn [الدالة](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) العثور على المحتوى الذي يطابق النمط.

  - تم العثور على كلمة رئيسية من [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) ومن أمثلة الكلمات الرئيسية: *الضمان الاجتماعي، الضمان الاجتماعي#، Soc Sec، SSN* . على سبيل المثال، سيتم تشغيل العينة التالية لسياسة DLP SSN: **SSN: 489-36-8350**
  
لمزيد من المعلومات حول ما هو مطلوب لSSNs ليتم الكشف عن المحتوى الخاص بك، راجع المقطع التالي في هذه المقالة: [ما أنواع المعلومات الحساسة البحث عن SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
باستخدام نوع معلومات حساسة مضمن ة مختلفة، راجع المقالة التالية للحصول على معلومات حول ما هو مطلوب للأنواع الأخرى: [ما تبحث عنه أنواع المعلومات الحساسة](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  