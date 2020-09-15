---
title: قاعده DLP لرقم حساب مصرفي الولايات المتحدة لا يعمل
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679283"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>مشاكل DLP مع أرقام الحسابات المصرفية في الولايات المتحدة

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

**مشاكل DLP مع أرقام الحسابات المصرفية في الولايات المتحدة**

هل تواجه مشاكل متعلقة **بمنع فقدان البيانات (DLP)** لا تعمل علي المحتوي الذي يحتوي علي **رقم حساب مصرفي للولايات** المتحدة عند استخدام نوع المعلومات الحساسة ل DLP في O365 ؟ إذا كان الأمر كذلك ، فتاكد من ان المحتوي يحتوي علي المعلومات المطلوبة لما يبحث عنه نهج DLP عند تقييمه.
  
علي سبيل المثال ، بالنسبة لنهج **رقم حساب مصرفي للولايات** المتحدة تم تكوينه باستخدام مستوي الثقة في 85% ، يتم تقييم التالي ويجب الكشف عنه لكي يتم تشغيل القاعدة:
  
- **[التنسيق:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 أرقام

- **[النمط:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 أرقاما متتالية.

- **[المجموع الاختباري:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** لا ، لا توجد مجموعات اختباريه

- **[تعريف:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** نهج DLP هو 75% تثق بأنه قد تم اكتشاف هذا النوع من المعلومات الهامه في حال وجوده في غضون أكثر من 300 حرفا:

  - يبحث التعبير العادي Regex_usa_bank_account_number عن المحتوي الذي يتطابق مع النمط

  - تم العثور علي كلمه أساسيه من Keyword_usa_Bank_Account.

    علي سبيل المثال ، سيتم تشغيل النموذج التالي لنهج **رقم الحساب المصرفي للولايات** المتحدة: التحقق من الحساب 78344011

للحصول علي مزيد من المعلومات حول ما هو مطلوب للحصول علي **رقم حساب مصرفي للولايات** المتحدة ، راجع القسم التالي في هذه المقالة: [ما الذي تبحث عنه أنواع المعلومات الهامه لرقم الحساب المصرفي الأمريكي](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
باستخدام نوع آخر من المعلومات الحساسة المضمنة ، راجع المقالة التالية للحصول علي معلومات حول ما هو مطلوب للأنواع الأخرى: [ما الذي تبحث عنه أنواع المعلومات الهامه](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  