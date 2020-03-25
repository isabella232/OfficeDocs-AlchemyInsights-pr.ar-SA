---
title: لا يمكن تسجيل الدخول إلى Teams بسبب الخطأ autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931766"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>لا يمكن تسجيل الدخول إلى Teams بسبب الخطأ autologon.microsoftazuread-sso dot com:443

إذا تم تمكين SSO كمصادقة لـ O365، فقد تحتاج إلى إضافة عنوان URL "autologon.microsoftazuread-sso.com" إلى مواقع الإنترانت.  إذا تمت إضافته إلى "المواقع الموثوق بها" مسبقاً وكان SSO قيد الاستخدام، فيجب إزالته من "المواقع الموثوق بها".

الرجاء مراجعة["قائمة اختيار استكشاف أخطاء SSO وإصلاحها"](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

اتبع هذه الخطوات لإضافة عنوان URL إلى قائمة مواقع الإنترانت:

1. افتح Internet Explorer بالنقر فوق الزر **"بدء"**. في مربع البحث اكتب Internet Explorer، ثم انقر فوق **Internet Explorer**في قائمة النتائج.
2. انقر فوق قائمة **أدوات** ثم انقر فوق **خيارات الإنترنت**.
3. انقر فوق علامة التبويب **أمان**.
4. انقر الآن فوق **مواقع إنترانت المحلية** ثم انقر فوق الزر **المواقع** ثم فوق الزر **متقدم**.
5. ادخل عنوان URL لموقع الويب ثم انقر فوق **"إضافة"**.
6. عند الانتهاء، انقر فوق **إغلاق**.

للحصول على مزيد من المعلومات، راجع [وثائق لنشر SSO لـ O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (يتضمن العملية المستندة إلى النهج لإضافة عنوان URL إلى مواقع إنترانت في الخطوة 3).
