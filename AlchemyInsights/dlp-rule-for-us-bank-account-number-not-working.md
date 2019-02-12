---
title: قاعدة DLP "لنا رقم الحساب البنكي" لا يعمل
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916403"
---
هل تواجه مشاكل في **منع فقدان البيانات (DLP)** لا يعمل للمحتوى الذي يحتوي على **رقم الحساب البنكي الولايات المتحدة** عند استخدام نوع معلومات حساسة DLP في O365؟ إذا كان الأمر كذلك، تأكد من أن المحتوى الخاص بك يحتوي على المعلومات المطلوبة لما نهج DLP تبحث عنه عندما يتم تقييم. 
  
على سبيل المثال، لنهج **الولايات المتحدة رقم الحساب البنكي** الذي تم تكوينه بمستوى ثقة 85%، التالية يتم تقييمها ويجب الكشف عن لتشغيل القاعدة: 
  
- **[تنسيق:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** أرقام 8 17 
    
- **[نمط:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** رقم 8-17 على التوالي. 
    
- **[المجموع الاختباري:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** لا، هناك لم المجموع الاختباري 
    
- **[تعريف:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** نهج DLP هي 75% واثقاً من الكشف عن هذا النوع من المعلومات الهامة إذا مسافة 300 حرف: 
    
  - التعبير العادي Regex_usa_bank_account_number البحث عن المحتوى الذي يطابق نمط
    
  - تم العثور على كلمة أساسية من Keyword_usa_Bank_Account.
    
    على سبيل المثال، فسيتم تشغيل النموذج التالي للسياسة **الأمريكية رقم الحساب البنكي** : 78344011 التحقق من الحساب 
    
لمزيد من المعلومات حول ما هو مطلوب **رقم الحساب البنكي في الولايات المتحدة** بأن يتم كشفه للمحتوى، راجع المقطع التالي في هذا المقال: [ما الحساسة معلومات الأنواع ابحث عن "رقم الحساب البنكي في الولايات المتحدة"](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
استخدام نوع معلومات حساسة مضمنة مختلفة، راجع المقالة التالية للحصول على المعلومات على ما هو مطلوب للأنواع الأخرى: [البحث عن "ما الحساسة معلومات الأنواع"](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

