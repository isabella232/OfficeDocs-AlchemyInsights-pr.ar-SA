---
title: دلب قاعدة للولايات المتحدة/"المملكة المتحدة رقم جواز السفر" لا يعمل
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bc91af8be58d49204f84cd7d22f481348af3c013
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529906"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>مشاكل تقنية DLP-الولايات المتحدة/المملكة المتحدة رقم جواز السفر

هل تواجه مشاكل **منع فقدان البيانات (DLP)** لا يعمل لاحتواء المحتوى **الولايات المتحدة/"المملكة المتحدة رقم جواز السفر"** عند استخدام نوع معلومات حساسة DLP في O365؟ إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لما نهج DLP تبحث عنه عندما يتم تقييم.
  
على سبيل المثال، **الولايات المتحدة/"المملكة المتحدة رقم جواز السفر"** النهج المكون بمستوى ثقة 75%، التالية يتم تقييمها ويجب الكشف عن لتشغيل القاعدة
  
- **[تنسيق:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** تسعة أرقام

- **[نموذج:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** تسعة أرقام متتالية

- **[المجموع الاختباري:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** لا، هناك لم المجموع الاختباري

- **[تعريف:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** نهج DLP هي 75% واثقاً من الكشف عن هذا النوع من المعلومات الهامة إذا مسافة 300 حرف:

  - دالة Func_usa_uk_passport البحث عن المحتوى الذي يطابق النموذج.

  - تم العثور على كلمة أساسية من Keyword_passport.

    على سبيل المثال، فسيتم تشغيل النموذج التالي **الولايات المتحدة/"المملكة المتحدة رقم جواز السفر"** النهج: رقم "جواز السفر الأمريكي" 123456789

لمزيد من المعلومات حول ما هو مطلوب للولايات المتحدة/"رقم جواز السفر المملكة المتحدة" بأن يتم كشفه للمحتوى، راجع المقطع التالي في هذه المقالة: [مظهر "ما الحساسة معلومات الأنواع" للولايات المتحدة/"المملكة المتحدة رقم جواز السفر"](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
استخدام نوع معلومات حساسة مضمنة مختلفة، راجع المقالة التالية للحصول على المعلومات على ما هو مطلوب للأنواع الأخرى: [البحث عن "ما الحساسة معلومات الأنواع"](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  