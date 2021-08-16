---
title: قاعدة DLP لرقم جواز سفر الولايات المتحدة/المملكة المتحدة لا تعمل
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
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004933"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>مشاكل في DLP - أرقام جواز سفر الولايات المتحدة والمملكة المتحدة

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

**مشاكل DLP مع أرقام جواز سفر الولايات المتحدة والمملكة المتحدة**

هل تواجه مشاكل في منع فقدان البيانات **(DLP)** لا تعمل على محتوى يحتوي على رقم جواز سفر **أمريكي/المملكة** المتحدة عند استخدام نوع معلومات حساسة ل DLP في O365؟ إذا كان الأمر كذلك، فتأكد من أن المحتوى يحتوي على المعلومات المطلوبة حول ما يبحث عنه نهج DLP عند تقييمه.
  
على سبيل المثال، بالنسبة إلى نهج رقم جواز سفر الولايات المتحدة **والمملكة** المتحدة الذي تم تكوينه بمستوى ثقة بنسبة 75٪، يتم تقييم ما يلي ويجب اكتشافه حتى يتم تشغيل القاعدة
  
- **[التنسيق:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** تسعة أرقام

- **[النمط:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** تسعة أرقام متتالية

- **[الاختبارات:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** لا، لا يوجد "شيكوم"

- **[التعريف:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** إن نهج DLP واثق بنسبة 75٪ من أنه تم الكشف عن هذا النوع من المعلومات الحساسة إذا، ضمن تقارب 300 حرف:

  - تعثر الدالة Func_usa_uk_passport المحتوى الذي يتطابق مع النمط.

  - تم العثور على كلمة أساسية Keyword_passport كلمة أساسية.

    على سبيل المثال، قد يتم تشغيل العينة التالية لسياسة رقم جواز سفر الولايات **المتحدة/المملكة** المتحدة: رقم جواز السفر 123456789

للحصول على مزيد من المعلومات حول ما هو مطلوب لرقم جواز سفر الولايات المتحدة/المملكة المتحدة للكشف عن المحتوى الخاص بك، راجع القسم التالي في هذه المقالة: ما تبحث عنه أنواع المعلومات الحساسة لرقم جواز سفر الولايات [المتحدة/المملكة المتحدة](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
باستخدام نوع مختلف من المعلومات الحساسة المضمنة، راجع المقالة التالية للحصول على معلومات حول ما هو مطلوب للأنواع الأخرى: ما تبحث عنه أنواع المعلومات [الحساسة](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  