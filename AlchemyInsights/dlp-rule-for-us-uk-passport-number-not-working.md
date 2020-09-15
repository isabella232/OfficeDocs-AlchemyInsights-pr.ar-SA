---
title: قاعده DLP لرقم Passport للولايات المتحدة/المملكة المتحدة لا يعمل
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679211"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>المشاكل المتعلقة بأرقام passport للولايات المتحدة/المملكة المتحدة

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

**مشاكل DLP مع أرقام passport الامريكيه/المملكة المتحدة**

هل تواجه مشاكل متعلقة **بمنع فقدان البيانات (DLP)** لا تعمل علي المحتوي الذي يحتوي علي **رقم passport للولايات المتحدة/المملكة** المتحدة عند استخدام نوع المعلومات الحساسة ل DLP في O365 ؟ إذا كان الأمر كذلك ، فتاكد من ان المحتوي يحتوي علي المعلومات المطلوبة لما يبحث عنه نهج DLP عند تقييمه.
  
علي سبيل المثال ، بالنسبة إلى نهج **رقم passport للولايات المتحدة/المملكة** المتحدة المكون بمستوي الثقة في 75% ، يتم تقييم التالي ويجب الكشف عنه لكي يتم تشغيل القاعدة
  
- **[تنسيق:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** تسعه أرقام

- **[النمط:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** تسعه أرقام متتالية

- **[المجموع الاختباري:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** لا ، لا توجد مجموعات اختباريه

- **[تعريف:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** نهج DLP هو 75% تثق بأنه قد تم اكتشاف هذا النوع من المعلومات الهامه في حال وجوده في غضون أكثر من 300 حرفا:

  - تعثر الدالة Func_usa_uk_passport علي المحتوي الذي يتطابق مع النمط.

  - تم العثور علي كلمه أساسيه من Keyword_passport.

    علي سبيل المثال ، سيتم تشغيل النموذج التالي لسياسة **رقم passport الامريكيه/المملكة** المتحدة: رقم passport الأمريكي 123456789

للحصول علي مزيد من المعلومات حول العناصر المطلوبة للحصول علي رقم Passport للولايات المتحدة/المملكة المتحدة ، راجع القسم التالي في هذه المقالة: [ما الذي تبحث عنه أنواع المعلومات الهامه لرقم الولايات المتحدة/المملكة المتحدة](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
باستخدام نوع آخر من المعلومات الحساسة المضمنة ، راجع المقالة التالية للحصول علي معلومات حول ما هو مطلوب للأنواع الأخرى: [ما الذي تبحث عنه أنواع المعلومات الهامه](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  