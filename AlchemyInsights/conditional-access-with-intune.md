---
title: الوصول الشرطي باستخدام Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069699"
---
# <a name="conditional-access-with-intune"></a>الوصول الشرطي باستخدام Intune

يتطلب  **استخدام الوصول**  الشرطي مع Intune 3 خطوات:

- إنشاء نهج **التوافق** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android) [وiOS](https://docs.microsoft.com/intune/compliance-policy-create-ios) [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) لتحديد الإعدادات التي يجب أن يتم التحقق من مطابقتها قبل أن يعتبر الجهاز متوافقا. على سبيل المثال، يجب أن يكون لدى الجهاز دبوس من 6 أرقام على الأقل قبل أن يعتبر متوافقا.
- أنشئ نهج **الوصول الشرطي**  الذي يحدد الموارد التي يتم حمايتها، والشروط التي يجب أن يتم توفيرها للوصول إلى تلك الموارد.  [على سبيل المثال،](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  يجب أن يكون الجهاز متوافقا قبل الوصول إلى البريد الإلكتروني الخاص بالشركة.
- تأكد من أن كل من **"سياسات**  التوافق" و"سياسات  **الوصول**  الشرطي" تستهدف مجموعات المستخدمين المطلوبة. قد يتطلب ذلك إنشاء مجموعات معينة من المستخدمين في Azure Active Directory.

**ارتباطات مفيدة:**

[نظرة عامة حول توافق الجهاز](https://docs.microsoft.com/intune/device-compliance-get-started)

[استكشاف الأخطاء الم CA وإصلاحها](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[نهج استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

لحماية البريد الإلكتروني (Exchange الإنترنت) من الوصول بواسطة الأجهزة غير المتوافقة، يجب اتباع المستندين:

1. [حماية الوصول إلى البريد الإلكتروني من الأجهزة التي تستخدم EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [حماية الوصول إلى البريد الإلكتروني من الأجهزة باستخدام عملاء المصادقة الحديثة مثل Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)