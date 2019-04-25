---
title: دلب قاعدة للتأمين الاجتماعي لا يعمل
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: d2d21fb5546d36990d69b76e3ceb72ce2edf3d80
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404404"
---
هل تواجه مشاكل في **منع فقدان البيانات (DLP)** لا يعمل للمحتوى الذي يحتوي على **"رقم التأمين الاجتماعي" (SSN)** عند استخدام نوع معلومات حساسة في Office 365؟ إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لما يبحث النهج DLP. 
  
على سبيل المثال، لنهج التأمين الاجتماعي تكوين بمستوى ثقة 85%، التالية يتم تقييمها ويجب الكشف عن لتشغيل القاعدة:
  
- **[التنسيق:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 أرقام، الذي قد يكون في نمط منسق أو غير منسق 
    
- **[نموذج:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** أربع مهام البحث عن شبكات الأمان الاجتماعي في أربعة أنماط مختلفة: 
    
  - Func_ssn البحث عن شبكات الأمان الاجتماعي ب 2011 قبل تنسيق قوي المنسقة بواسطة شرطات أو مسافات (dddd dd ddd أو ddd يوم dddd)
    
  - Func_unformatted_ssn البحث عن شبكات الأمان الاجتماعي ب 2011 قبل تنسيق قوي التي تكون غير منسقة تسعة أرقام متتالية (دددددددد)
    
  - ويرى Func_randomized_formatted_ssn 2011 نشر شبكات الأمان الاجتماعي التي تم تنسيقها باستخدام الشرط أو مسافات (dddd dd ddd أو ddd يوم dddd)
    
  - ويرى Func_randomized_unformatted_ssn 2011 نشر شبكات الأمان الاجتماعي التي تكون غير منسقة تسعة أرقام متتالية (دددددددد)
    
- **[المجموع الاختباري:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** لا، هناك لم المجموع الاختباري 
    
- **[تعريف:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** هو نهج DLP 85% واثقاً من الكشف عن هذا النوع من المعلومات الهامة إذا مسافة 300 حرف: 
    
  - [دالة Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) البحث عن المحتوى الذي يطابق النموذج. 
    
  - تم العثور على كلمة أساسية من [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . تتضمن أمثلة للكلمات الأساسية: *الضمان الاجتماعي، # الضمان الاجتماعي، شركة نفط الجنوب الثانية، والتأمين الاجتماعي* . على سبيل المثال، فسيتم تشغيل النموذج التالي لنهج التأمين الاجتماعي DLP: **رقم الضمان الاجتماعي: 489-36-8350**
    
لمزيد من المعلومات حول ما هو مطلوب لشبكات الأمان الاجتماعي بأن يتم كشفه للمحتوى، راجع المقطع التالي في هذا المقال: [ما الحساسة معلومات الأنواع البحث عن شبكات الأمان الاجتماعي](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
استخدام نوع معلومات حساسة مضمنة مختلفة، راجع المقالة التالية للحصول على المعلومات على ما هو مطلوب للأنواع الأخرى: [البحث عن "ما الحساسة معلومات الأنواع"](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

