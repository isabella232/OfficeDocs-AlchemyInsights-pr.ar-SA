---
title: DLP لا يعمل كما هو متوقع
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
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079689"
---
# <a name="dlp-not-working-as-expected"></a>DLP لا يعمل كما هو متوقع

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

 **إعداد DLP**

هل تواجه مشاكل في منع فقدان البيانات **(DLP)** Office 365 تعمل كما هو متوقع؟ إذا كان الأمر كذلك، فتأكد من إعداد نهج **DLP** بشكل صحيح، ومن احتواء بياناتك على ما يبحث عنه نهج **DLP** عند تقييمه.
  
تسمح لك سياسات DLP بتحديد المعلومات الحساسة وحمايتها في مؤسستك. لإعداد سياسات DLP، استخدم المعلومات [هنا](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).
  
 **ما تبحث عنه سياسات DLP**
  
عند استخدام **أنواع** المعلومات الحساسة المضمنة في مراكز الأمان والتوافق، تبحث سياسات DLP عن أنماط وعناصر معينة عند الكشف عن هذه الأنواع الحساسة.
  
- **أنواع المعلومات الحساسة المضمنة**

    للحصول على معلومات حول الأنواع الحساسة المضمنة وما تبحث عنه نهج DLP عند الكشف عن النوع الحساس، راجع: ما تبحث عنه أنواع المعلومات [الحساسة.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **أنواع المعلومات الحساسة المخصصة**

    إذا كنت تحاول إنشاء أنواع معلومات حساسة مخصصة، فاستخدم المقالة التالية للحصول على معلومات حول كيفية إنشاء نوع مخصص حساس: إنشاء نوع معلومات [مخصص حساس](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**اختبار نهج DLP**

لاختبار البيانات باستخدام نوع معلومات حساسة مضمن أو  مخصص، استخدم الخيار نوع الاختبار ضمن أنواع المعلومات **الحساسة**  >  **للتصنيفات**. لمزيد من المعلومات، راجع [اختبار أنواع المعلومات الحساسة المخصصة](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **التقارير**
  
- احصل على تحليلات البيانات الحساسة باستخدام [تقارير DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- راجع تفاصيل معينة للحدث باستخدام تقرير [حادث](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
