---
title: قاعدة DLP ل SSN لا تعمل
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004969"
---
# <a name="dlp-issues-with-social-security-numbers"></a>مشاكل DLP مع أرقام الضمان الاجتماعي

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

**مشاكل DLP مع SSNs**

هل تواجه مشاكل في منع فقدان البيانات **(DLP)** لا تعمل مع المحتوى الذي يحتوي على رقم الضمان الاجتماعي **(SSN)** عند استخدام نوع معلومات حساسة في Microsoft 365؟ إذا كان الأمر كذلك، فتأكد من أن المحتوى يحتوي على المعلومات المطلوبة حول المظهر الذي يبحث عنه نهج DLP. 
  
على سبيل المثال، بالنسبة إلى نهج SSN الذي تم تكوينه بمستوى ثقة 85٪، يتم تقييم ما يلي ويجب اكتشافه حتى يتم تشغيل القاعدة:
  
- **[التنسيق:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 أرقام، والتي قد تكون في نمط تم تنسيقه أو غير تنسيقه

- **[النمط:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** تبحث أربع دالات عن SSN في أربعة أنماط مختلفة:

  - Func_ssn البحث عن SSN بتنسيق قوي قبل 2011 تم تنسيقه باستخدام شرط أو مسافات (ddd-dddd أو ddd ddd ddddd)

  - Func_unformatted_ssn البحث عن SSN بتنسيق قوي قبل 2011 غير منسق بتسعة أرقام متتالية (dddddddddd)

  - Func_randomized_formatted_ssn البحث عن SSN بعد عام 2011 التي تم تنسيقها باستخدام شرط أو مسافات (ddd-ddddD OR ddd ddddd)

  - Func_randomized_unformatted_ssn البحث عن SSN بعد 2011 التي لم يتم فرزها بتسعة أرقام متتالية (ddddddddd)

- **[الاختبارات:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** لا، لا يوجد "شيكوم"

- **[التعريف:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** إن نهج DLP واثق بنسبة 85٪ من أنه تم الكشف عن هذا النوع من المعلومات الحساسة إذا، ضمن تقارب 300 حرف:

  - تعثر [الدالة Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) المحتوى الذي يتطابق مع النمط.

  - تم العثور على [كلمة أساسية من](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) Keyword_ssn. تتضمن أمثلة الكلمات الأساسية:  *الضمان الاجتماعي، الضمان الاجتماعي#، Soc Sec ، SSN*  . على سبيل المثال، قد يتم تشغيل العينة التالية لن نهج DLP SSN: **SSN: 489-36-8350**
  
للحصول على مزيد من المعلومات حول ما هو مطلوب للكشف عن SSNs لمحتواك، راجع المقطع التالي في هذه المقالة: ما تبحث عنه أنواع المعلومات الحساسة [ل SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
باستخدام نوع مختلف من المعلومات الحساسة المضمنة، راجع المقالة التالية للحصول على معلومات حول ما هو مطلوب للأنواع الأخرى: ما تبحث عنه أنواع المعلومات [الحساسة](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  