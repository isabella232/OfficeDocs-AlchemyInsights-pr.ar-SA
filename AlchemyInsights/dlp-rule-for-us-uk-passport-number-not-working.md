---
title: دلب قاعدة للولايات المتحدة/"المملكة المتحدة رقم جواز السفر" لا يعمل
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29455980"
---
هل تواجه مشاكل **منع فقدان البيانات (DLP)** لا يعمل لاحتواء المحتوى **الولايات المتحدة/"المملكة المتحدة رقم جواز السفر"** عند استخدام نوع معلومات حساسة DLP في O365؟ إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لما نهج DLP تبحث عنه عندما يتم تقييم. 
  
على سبيل المثال، **الولايات المتحدة/"المملكة المتحدة رقم جواز السفر"** النهج المكون بمستوى ثقة 75%، التالية يتم تقييمها ويجب الكشف عن لتشغيل القاعدة 
  
- **[تنسيق:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** تسعة أرقام 
    
- **[نموذج:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** تسعة أرقام متتالية 
    
- **[المجموع الاختباري:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** لا، هناك لم المجموع الاختباري 
    
- **[تعريف:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** نهج DLP هي 75% واثقاً من الكشف عن هذا النوع من المعلومات الهامة إذا مسافة 300 حرف: 
    
  - دالة Func_usa_uk_passport البحث عن المحتوى الذي يطابق النموذج.
    
  - تم العثور على كلمة أساسية من Keyword_passport.
    
    على سبيل المثال، فسيتم تشغيل النموذج التالي **الولايات المتحدة/"المملكة المتحدة رقم جواز السفر"** النهج: رقم "جواز السفر الأمريكي" 123456789 
    
لمزيد من المعلومات حول ما هو مطلوب للولايات المتحدة/"رقم جواز السفر المملكة المتحدة" بأن يتم كشفه للمحتوى، راجع المقطع التالي في هذه المقالة: [مظهر "ما الحساسة معلومات الأنواع" للولايات المتحدة/"المملكة المتحدة رقم جواز السفر"](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
استخدام نوع معلومات حساسة مضمنة مختلفة، راجع المقالة التالية للحصول على المعلومات على ما هو مطلوب للأنواع الأخرى: [البحث عن "ما الحساسة معلومات الأنواع"](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

