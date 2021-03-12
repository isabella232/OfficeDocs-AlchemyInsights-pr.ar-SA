---
title: لا تعمل DLP كما هو متوقع
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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707797"
---
# <a name="dlp-not-working-as-expected"></a>لا تعمل DLP كما هو متوقع

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

 **إعداد DLP**

هل تواجه مشاكل في منع فقدان **البيانات (DLP)** في Office 365 لا يعمل كما هو متوقع؟ إذا كان الأمر كذلك، فتأكد من إعداد نهج **DLP** بشكل صحيح، ومن احتواء بياناتك على ما يبحث عنه نهج **DLP** عند تقييمه.
  
تسمح لك سياسات DLP بتحديد المعلومات الحساسة في مؤسستك وحمايتها. لإعداد سياسات DLP، استخدم المعلومات [هنا.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **ما تبحث عنه سياسات DLP**
  
عند استخدام أنواع **المعلومات** الحساسة المضمنة في مراكز الأمان والتوافق، تبحث سياسات DLP عن أنماط وعناصر معينة عند الكشف عن هذه الأنواع الحساسة.
  
- **أنواع المعلومات الحساسة المضمنة**

    للحصول على معلومات حول الأنواع الحساسة المضمنة وما الذي تبحث عنه سياسة DLP عند الكشف عن النوع الحساس، راجع: ما تبحث عنه أنواع المعلومات [الحساسة.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **أنواع المعلومات الحساسة المخصصة**

    إذا كنت تحاول إنشاء أنواع معلومات مخصصة حساسة، فاستخدم المقالة التالية للحصول على معلومات حول كيفية إنشاء نوع معلومات مخصص حساس: إنشاء نوع معلومات مخصص [حساس.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**اختبار نهج DLP**

لاختبار البيانات باستخدام نوع معلومات مضمن أو مخصص  حساس، استخدم الخيار "نوع الاختبار" ضمن أنواع المعلومات الحساسة  >  **للتصنيفات.** لمزيد من المعلومات، راجع [اختبار أنواع المعلومات الحساسة المخصصة.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **التقارير**
  
- احصل على تحليلات البيانات الحساسة باستخدام [تقارير DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- راجع تفاصيل معينة للحدث باستخدام تقرير [حادث.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
