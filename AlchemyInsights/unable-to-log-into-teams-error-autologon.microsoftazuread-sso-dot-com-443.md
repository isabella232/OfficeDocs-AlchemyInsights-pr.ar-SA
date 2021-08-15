---
title: لا يمكن تسجيل الدخول إلى Teams بسبب الخطأ autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038387"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>لا يمكن تسجيل الدخول إلى Teams بسبب الخطأ autologon.microsoftazuread-sso dot com:443

إذا تم تمكين SSO كمصادقة لـ O365، فقد تحتاج إلى إضافة عنوان URL "autologon.microsoftazuread-sso.com" إلى مواقع الإنترانت.  إذا تمت إضافته إلى "المواقع الموثوق بها" مسبقاً وكان SSO قيد الاستخدام، فيجب إزالته من "المواقع الموثوق بها".

الرجاء مراجعة["قائمة اختيار استكشاف أخطاء SSO وإصلاحها"](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

اتبع هذه الخطوات لإضافة عنوان URL إلى قائمة مواقع الإنترانت:

1. افتح Internet Explorer بالنقر فوق الزر **"بدء"**. في مربع البحث اكتب Internet Explorer، ثم انقر فوق **Internet Explorer** في قائمة النتائج.
2. انقر فوق قائمة **أدوات** ثم انقر فوق **خيارات الإنترنت**.
3. انقر فوق علامة التبويب **أمان**.
4. انقر الآن فوق **مواقع إنترانت المحلية** ثم انقر فوق الزر **المواقع** ثم فوق الزر **متقدم**.
5. ادخل عنوان URL لموقع الويب ثم انقر فوق **"إضافة"**.
6. عند الانتهاء، انقر فوق **إغلاق**.

للحصول على مزيد من المعلومات، راجع [وثائق لنشر SSO لـ O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (يتضمن العملية المستندة إلى النهج لإضافة عنوان URL إلى مواقع إنترانت في الخطوة 3).
