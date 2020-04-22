---
title: قاعدة DLP لرقم الحساب المصرفي الأمريكي لا يعمل
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 45aa50f6c3505468e902e58faf698205f93f9264
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704026"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>إصدارات DLP مع أرقام الحسابات المصرفية في الولايات المتحدة

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

**إصدارات DLP مع أرقام الحسابات المصرفية في الولايات المتحدة**

هل تواجه مشاكل مع **منع فقدان البيانات (DLP)** لا تعمل للمحتوى الذي يحتوي على **رقم حساب مصرفي في الولايات المتحدة** عند استخدام نوع معلومات حساسة DLP في O365؟ إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لما تبحث عنه سياسة DLP عند تقييمه.
  
على سبيل المثال، بالنسبة لسياسة **رقم الحساب المصرفي الأمريكي** التي تم تكوينها بمستوى ثقة 85%، يتم تقييم ما يلي ويجب الكشف عنها حتى تقوم القاعدة بتشغيلها:
  
- **[الشكل:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 أرقام

- **[النمط:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 أرقام متتالية.

- **[المجموع الاختياري:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** لا، لا يوجد المجموع الاختياري

- **[التعريف:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** سياسة DLP واثقة بنسبة 75٪ من أنها اكتشفت هذا النوع من المعلومات الحساسة إذا، على مقربة من 300 حرف:

  - Regex_usa_bank_account_number التعبير العادي يبحث عن المحتوى الذي يطابق النمط

  - تم العثور على كلمة رئيسية من Keyword_usa_Bank_Account.

    على سبيل المثال، سيتم تشغيل العينة التالية لسياسة **رقم الحساب المصرفي الأمريكي:** التحقق من الحساب 78344011

لمزيد من المعلومات حول ما هو مطلوب للكشف عن **رقم الحساب المصرفي الأمريكي** للمحتوى الخاص بك، راجع القسم التالي في هذه المقالة: ما أنواع المعلومات [الحساسة البحث عن رقم الحساب المصرفي الأمريكي](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
باستخدام نوع معلومات حساسة مضمن ة مختلفة، راجع المقالة التالية للحصول على معلومات حول ما هو مطلوب للأنواع الأخرى: [ما تبحث عنه أنواع المعلومات الحساسة](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  