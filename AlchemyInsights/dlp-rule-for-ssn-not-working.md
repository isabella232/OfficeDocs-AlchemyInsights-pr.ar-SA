---
title: قاعدة DLP لـ SSN لا تعمل
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 5af843c2b70b5b2e1aaf82c9f01356546929d840
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43788689"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP القضايا مع أرقام الضمان الاجتماعي

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

**مشكلات DLP مع SSNs**

هل تواجه مشاكل مع **منع فقدان البيانات (DLP)** لا تعمل للمحتوى الذي يحتوي على **رقم الضمان الاجتماعي (SSN)** عند استخدام نوع معلومات حساسة في Microsoft 365؟ إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لما تبحث عنه سياسة DLP. 
  
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
  