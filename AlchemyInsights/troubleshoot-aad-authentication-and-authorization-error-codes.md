---
title: استكشاف أخطاء رموز الخطأ مصادقة Azure AD وتخويلها (AADSTS) وإصلاحها
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034845"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>استكشاف أخطاء رموز الخطأ مصادقة Azure AD وتخويلها (AADSTS) وإصلاحها

لحل رموز أخطاء مصادقة AAD وتخويلها (AADSTS)، يجب تنفيذ الخطوات التالية الموصى بها:

1. **معالجة رموز الخطأ في التطبيق**

- يوفر **المواصفات OAuth2.0**، إرشادات حول كيفية معالجة الأخطاء أثناء المصادقة باستخدام جزء الخطأ https://tools.ietf.org/html/rfc6749#section-5.2 من استجابة الخطأ.

    - **:** سلسلة رمز خطأ يمكن استخدامها لتصنيف أنواع الأخطاء التي تحدث، ويجب استخدامها للتفاعل مع الأخطاء.
    - حقل **الخطأ** له عدة قيم محتملة - راجع ارتباطات وثائق البروتوكول والمواصفات OAuth 2.0 للحصول على مزيد من المعلومات حول أخطاء معينة وكيفية التفاعل معها.

- فيما يلي استجابة نموذجية للخطأ:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **البحث عن معلومات رمز الخطأ الحالي**

- رموز الأخطاء والرسائل عرضة للتغيير. للحصول على أحدث المعلومات، راجع الصفحة للعثور على أوصاف أخطاء AADSTS وإصلاحاتها وبعض الحلول https://login.microsoftonline.com/error المقترحة.
- يمكنك أيضا البحث عن رموز أخطاء [AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) المدرجة في المقالة مصادقة Azure AD ورموز خطأ [التخويل وإصلاحها.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)

3. **الحصول على تعليمات**

- [خيارات الدعم والدعم](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) للمطورين - إذا كنت بحاجة إلى إجابة عن سؤال أو مساعدة لحل مشكلة غير مشمولة في وثائقنا، فقد يكون الوقت قد حان للوصول إلى الخبراء للحصول على المساعدة. توفر هذه المقالة العديد من الاقتراحات للحصول على إجابات لأسئلتك عند تطوير التطبيقات التي تتكامل مع النظام الأساسي لهوية Microsoft.








