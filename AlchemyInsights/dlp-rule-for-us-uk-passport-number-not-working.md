---
title: قاعدة DLP لرقم جواز السفر الأمريكي /UK لا يعمل
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507285"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>مشاكل مع DLP - أرقام جوازات السفر الأمريكية /المملكة المتحدة

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

**DLP القضايا مع أرقام جوازات السفر الأمريكية / المملكة المتحدة**

هل تواجه مشاكل مع **منع فقدان البيانات (DLP)** لا تعمل للمحتوى الذي يحتوي على **رقم جواز سفر الولايات المتحدة / المملكة المتحدة** عند استخدام نوع معلومات حساسة DLP في O365؟ إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لما تبحث عنه سياسة DLP عند تقييمه.
  
على سبيل المثال، بالنسبة لسياسة **رقم جواز سفر الولايات المتحدة والمملكة المتحدة** التي تم تكوينها بمستوى ثقة 75٪، يتم تقييم ما يلي ويجب الكشف عنها لتشغيل القاعدة
  
- **[الشكل:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** تسعة أرقام

- **[نمط:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** تسعة أرقام متتالية

- **[المجموع الاختياري:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** لا، لا يوجد المجموع الاختياري

- **[التعريف:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** سياسة DLP واثقة بنسبة 75٪ من أنها اكتشفت هذا النوع من المعلومات الحساسة إذا، على مقربة من 300 حرف:

  - Func_usa_uk_passport تعثر الدالة على المحتوى الذي يطابق النقش.

  - تم العثور على كلمة رئيسية من Keyword_passport.

    على سبيل المثال، ستثير العينة التالية سياسة **رقم جواز السفر الأمريكي/المملكة المتحدة:** رقم جواز السفر الأمريكي 123456789

لمزيد من المعلومات حول ما هو مطلوب للكشف عن رقم جواز سفر الولايات المتحدة والمملكة المتحدة للمحتوى الخاص بك، راجع القسم التالي في هذه المقالة: [ما أنواع المعلومات الحساسة البحث عن رقم جواز سفر الولايات المتحدة / المملكة المتحدة](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
باستخدام نوع معلومات حساسة مضمن ة مختلفة، راجع المقالة التالية للحصول على معلومات حول ما هو مطلوب للأنواع الأخرى: [ما تبحث عنه أنواع المعلومات الحساسة](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  