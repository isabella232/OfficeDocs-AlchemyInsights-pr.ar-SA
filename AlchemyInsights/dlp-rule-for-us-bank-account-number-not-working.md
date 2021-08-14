---
title: قاعدة DLP ل رقم الحساب البنكي الأميركي لا تعمل
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
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005005"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>مشاكل DLP مع أرقام الحسابات المصرفية الأمريكية

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

**مشاكل DLP مع أرقام الحسابات المصرفية الأمريكية**

هل تواجه مشاكل في منع فقدان البيانات **(DLP)** لا تعمل مع المحتوى الذي يحتوي على رقم حساب بنكي في الولايات المتحدة عند استخدام نوع معلومات حساسة ل DLP في O365؟  إذا كان الأمر كذلك، فتأكد من أن المحتوى يحتوي على المعلومات المطلوبة حول ما يبحث عنه نهج DLP عند تقييمه.
  
على سبيل المثال، بالنسبة إلى نهج رقم الحساب البنكي الأميركي الذي تم تكوينه بمستوى ثقة 85٪، يتم تقييم ما يلي ويجب اكتشافه حتى يتم تشغيل القاعدة: 
  
- **[التنسيق:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 رقما

- **[النمط:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 رقما متتاليا.

- **[الاختبارات:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** لا، لا يوجد "شيكوم"

- **[التعريف:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** إن نهج DLP واثق بنسبة 75٪ من أنه تم الكشف عن هذا النوع من المعلومات الحساسة إذا، ضمن تقارب 300 حرف:

  - يعثر التعبير Regex_usa_bank_account_number العادي على المحتوى الذي يتطابق مع النمط

  - تم العثور على كلمة أساسية Keyword_usa_Bank_Account كلمة أساسية.

    على سبيل المثال، قد يتم تشغيل العينة التالية لن نهج رقم الحساب **البنكي** الأميركي: التحقق من الحساب 78344011

لمزيد من المعلومات حول ما  هو مطلوب للكشف عن رقم حساب بنكي في الولايات المتحدة للمحتوى الخاص بك، راجع المقطع التالي في هذه [المقالة:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) ما تبحث عنه أنواع المعلومات الحساسة ل رقم الحساب البنكي الأميركي
  
باستخدام نوع مختلف من المعلومات الحساسة المضمنة، راجع المقالة التالية للحصول على معلومات حول ما هو مطلوب للأنواع الأخرى: ما تبحث عنه أنواع المعلومات [الحساسة](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  