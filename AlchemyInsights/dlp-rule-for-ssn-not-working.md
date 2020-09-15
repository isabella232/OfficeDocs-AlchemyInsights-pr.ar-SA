---
title: قاعده DLP لعدم العمل
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
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679356"
---
# <a name="dlp-issues-with-social-security-numbers"></a>مشاكل DLP مع أرقام الأمان الاجتماعي

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

**مشاكل DLP مع سنس**

هل تواجه مشاكل متعلقة **بمنع فقدان البيانات (DLP)** لا تعمل علي المحتوي الذي يحتوي علي **رقم الأمان الاجتماعي (SSN)** عند استخدام نوع معلومات حساس في Microsoft 365 ؟ إذا كان الأمر كذلك ، فتاكد من ان المحتوي يحتوي علي المعلومات المطلوبة لما تبحث عنه نهج DLP. 
  
علي سبيل المثال ، بالنسبة إلى نهج SSN تم تكوينه باستخدام مستوي الثقة في 85% ، يتم تقييم التالي ويجب الكشف عنه لكي يتم تشغيل القاعدة:
  
- **[تنسيق:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 أرقام ، والتي قد تكون بنمط منسق أو غير منسق

- **[النمط:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** تظهر أربعه دالات لسنس في أربعه نقوش مختلفه:

  - Func_ssn 2011 البحث عن السنس التي تم تنسيقها باستخدام الشرط أو المسافات (ddd-dd أو ddd إلى dddd)

  - Func_unformatted_ssn البحث عن السنس مع تنسيق 2011 القوي الذي تمت تهيئته علي انه تسعه أرقام متتالية (دددددددد)

  - تعثر الFunc_randomized_formatted_ssn علي 2011 سنس التي تم تنسيقها باستخدام الشرطات أو المسافات (ddd-dd أو ddd dd dddd)

  - تعثر الFunc_randomized_unformatted_ssn علي 2011 سنس التي تم تنسيقها علي انها تسعه أرقام متتالية (دددددددد)

- **[المجموع الاختباري:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** لا ، لا توجد مجموعات اختباريه

- **[تعريف:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** نهج DLP هو 85% تثق بأنه قد تم اكتشاف هذا النوع من المعلومات الهامه في حال وجوده في غضون أكثر من 300 حرفا:

  - تعثر [الدالة Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) علي المحتوي الذي يتطابق مع النمط.

  - تم العثور علي كلمه أساسيه من [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . تتضمن أمثله الكلمات  *الاساسيه: الأمان الاجتماعي ، الأمان الاجتماعي # ، Soc Sec ، SSN*  . علي سبيل المثال ، سيتم تشغيل النموذج التالي لنهج الاعداد الخاص ب DLP: **SSN: 489-36-8350**
  
للحصول علي مزيد من المعلومات حول العناصر المطلوبة لسنس التي سيتم الكشف عنها لمحتويك ، راجع القسم التالي في هذه المقالة: [ما الذي تبحث عنه أنواع المعلومات الهامه لسنس](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
باستخدام نوع آخر من المعلومات الحساسة المضمنة ، راجع المقالة التالية للحصول علي معلومات حول ما هو مطلوب للأنواع الأخرى: [ما الذي تبحث عنه أنواع المعلومات الهامه](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  