---
title: وصول شرطي باستخدام Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807646"
---
# <a name="conditional-access-with-intune"></a>وصول شرطي باستخدام Intune

يتطلب استخدام  **Access الشرطي**  مع Intune وجود 3 خطوات:

- أنشئ  **نهج توافق**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android)،  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios)،  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) لتحديد الإعدادات التي يجب استيفاءها قبل ان يتم اعتبار الجهاز متوافقا. علي سبيل المثال ، يجب ان يتوفر للجهاز رقم pin يتكون من 6 أرقام علي الأقل قبل ان يتم اعتباره متوافقا.
- قم بإنشاء **نهج وصول شرطي**  يحدد الموارد التي يتم حمايتها ، والشروط التي يجب استيفاءها للوصول إلى هذه الموارد.  [علي سبيل المثال ،](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  يجب ان يكون الجهاز متوافقا قبل الوصول إلى البريد الكتروني للشركة.
- تاكد من استهداف كل من **نهج التوافق**  **ونهج الوصول الشرطي**  لمجموعات المستخدمين المطلوبة. قد يتطلب ذلك إنشاء مجموعات معينه من المستخدمين في Azure Active directory.

**الارتباطات المفيدة:**

[نظره عامه علي توافق الاجهزه](https://docs.microsoft.com/intune/device-compliance-get-started)

[استكشاف أخطاء المراجع المصدقة](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[نهج استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

لحماية البريد الكتروني (Exchange online) من access بواسطة الاجهزه غير المتوافقة ، يجب اتباع كلا المستندين:

1. [حماية الوصول إلى البريد الكتروني من الاجهزه باستخدام EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [حماية الوصول إلى البريد الكتروني من الاجهزه باستخدام عملاء المصادقة الحديثة مثل Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)