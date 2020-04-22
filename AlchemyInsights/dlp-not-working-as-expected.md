---
title: DLP لا تعمل كما هو متوقع
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: efb4a19f345fe6b8a1e8bb72abeba4a923c05777
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704400"
---
# <a name="dlp-not-working-as-expected"></a>DLP لا تعمل كما هو متوقع

**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.

 **إعداد DLP**

هل تواجه مشاكل مع **منع فقدان البيانات (DLP)** في Office 365 لا يعمل كما هو متوقع؟ إذا كان الأمر كذلك، تأكد من إعداد **نهج DLP** بشكل صحيح، وأن بياناتك تحتوي على ما يبحث عنه **نهج DLP** عند تقييمه.
  
تسمح لك سياسات DLP بتحديد وحماية المعلومات الحساسة في مؤسستك. لإعداد نُهج DLP، استخدم المعلومات [هنا](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **ما تبحث عنه سياسات DLP**
  
عند استخدام **أنواع المعلومات الحساسة المضمنة** في مراكز الأمان والامتثال، تبحث نُهج DLP عن أنماط وعناصر محددة عند اكتشاف هذه الأنواع الحساسة.
  
- **أنواع المعلومات الحساسة المضمنة**

    للحصول على معلومات حول الأنواع الحساسة المضمنة وما يبحث عنه نهج DLP عند الكشف عن النوع الحساس، راجع: [ما تبحث عنه أنواع المعلومات الحساسة](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **أنواع المعلومات الحساسة المخصصة**

    إذا كنت تحاول إنشاء أنواع معلومات حساسة مخصصة، فاستخدم المقالة التالية للحصول على معلومات حول كيفية إنشاء نوع حساس مخصص: [إنشاء نوع معلومات حساسة مخصصة](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**اختبار نهج DLP**

لاختبار البيانات باستخدام نوع معلومات حساسة مضمنة أو مخصصة، استخدم خيار **نوع الاختبار** ضمن أنواع**المعلومات الحساسة** **للتصنيفات** > . لمزيد من المعلومات، راجع [اختبار أنواع المعلومات الحساسة المخصصة](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **التقارير**
  
- احصل على رؤى بيانات حساسة باستخدام [تقارير DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- راجع تفاصيل محددة للحدث مع [تقرير الحادث](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
