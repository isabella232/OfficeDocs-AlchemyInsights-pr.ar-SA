---
title: لا يعمل DLP كما هو متوقع
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679680"
---
# <a name="dlp-not-working-as-expected"></a>لا يعمل DLP كما هو متوقع

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

 **اعداد DLP**

هل تواجه مشاكل في **منع فقدان البيانات (DLP)** في Office 365 لا تعمل كما هو متوقع ؟ إذا كان الأمر كذلك ، فتاكد من اعداد **نهج dlp** بشكل صحيح ، ومن ان البيانات تحتوي علي ما تبحث عنه **نهج DLP** عند تقييمه.
  
تسمح لك نهج DLP بتعريف المعلومات الحساسة وحمايتها في مؤسستك. لاعداد نهج DLP ، استخدم المعلومات الموجودة [هنا](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **ما هي نهج DLP التي تبحث عنها**
  
عند استخدام **أنواع المعلومات الحساسة المضمنة** في مراكز الأمان والتوافق ، تبحث نهج DLP عن أنماط وعناصر معينه عند اكتشاف هذه الأنواع الحساسة.
  
- **أنواع المعلومات الحساسة المضمنة**

    للحصول علي معلومات حول الأنواع الحساسة المضمنة وما يبحث عنه نهج DLP عند اكتشاف النوع الحساس ، راجع: [ما الذي تبحث عنه أنواع المعلومات الهامه](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **أنواع المعلومات الحساسة المخصصة**

    إذا كنت تحاول إنشاء أنواع معلومات حساسة مخصصه ، فاستخدم المقالة التالية للحصول علي معلومات حول كيفيه إنشاء نوع حساس مخصص: [إنشاء نوع معلومات حساسة مخصصه](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**اختبار نهج DLP**

لاختبار البيانات باستخدام نوع معلومات حساس أو مخصص مضمن ، استخدم الخيار **نوع الاختبار** ضمن **تصنيف**  >  **أنواع المعلومات الحساسة**. لمزيد من المعلومات ، راجع [اختبار أنواع المعلومات الحساسة المخصصة](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **يراس**
  
- احصل علي معارف دقيقه للبيانات باستخدام [تقارير DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- راجع تفاصيل الحدث باستخدام [تقرير الحادث](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
