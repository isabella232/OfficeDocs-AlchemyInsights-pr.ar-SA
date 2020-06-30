---
title: الوصول المشروط مع Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931402"
---
# <a name="conditional-access-with-intune"></a>الوصول المشروط مع Intune

استخدام **"الوصول المشروط"** مع Intune يتطلب 3 خطوات:

- إنشاء **سياسة التوافق** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) لتحديد الإعدادات التي يجب تلبيتها قبل اعتبار الجهاز متوافقًا. على سبيل المثال، يجب أن يكون الجهاز دبوس من 6 أرقام على الأقل قبل أن يعتبر متوافقاً.
- إنشاء **نهج الوصول المشروط** الذي يحدد ما هي الموارد التي يتم حماية و الشروط التي يجب تلبيتها للوصول إلى تلك الموارد.  [على سبيل المثال،](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) يجب أن يكون الجهاز متوافقًا قبل الوصول إلى البريد الإلكتروني للشركة.
- تأكد من أن كلاً من **سياسات التوافق** وسياسات **الوصول المشروط** تستهدف مجموعات المستخدمين المطلوبة. قد يتطلب ذلك إنشاء مجموعات معينة من المستخدمين في "خدمة Active Directory Azure".

**روابط مفيدة:**

[نظرة عامة حول توافق الجهاز](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[نهج استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

لحماية البريد الإلكتروني (Exchange عبر الإنترنت) من الوصول من قبل الأجهزة غير المتوافقة، يجب اتباع كلا المستندين:

1. [حماية الوصول إلى البريد الإلكتروني من الأجهزة التي تستخدم EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [حماية الوصول إلى البريد الإلكتروني من الأجهزة التي تستخدم عملاء المصادقة الحديثة مثل Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)