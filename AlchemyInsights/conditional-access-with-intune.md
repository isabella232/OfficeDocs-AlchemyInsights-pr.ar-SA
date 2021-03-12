---
title: الوصول المشروط باستخدام Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704773"
---
# <a name="conditional-access-with-intune"></a>الوصول المشروط باستخدام Intune

يتطلب  **استخدام "الوصول المشروط"**  مع Intune ثلاث خطوات:

- قم بإنشاء  **نهج توافق**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android)أو  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios)أو  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)لتحديد الإعدادات التي يجب أن يتم التحقق من مطابقتها قبل أن يعتبر الجهاز متوافقا. على سبيل المثال، يجب أن يكون رقم pin في الجهاز 6 أرقام على الأقل قبل أن يعتبر متوافقا.
- أنشئ نهج **الوصول المشروط**  الذي يحدد الموارد التي يتم حمايتها، والشروط التي يجب أن يتم تأمينها للوصول إلى تلك الموارد.  [على سبيل المثال،](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  يجب أن يكون الجهاز متوافقا قبل الوصول إلى البريد الإلكتروني الخاص بالشركة.
- تأكد من **أن كل**  من "سياسات التوافق" و"سياسات  **الوصول**  المشروط" تستهدف مجموعات المستخدمين المطلوبة. قد يتطلب ذلك إنشاء مجموعات معينة من المستخدمين في Azure Active Directory.

**ارتباطات مفيدة:**

[نظرة عامة حول توافق الجهاز](https://docs.microsoft.com/intune/device-compliance-get-started)

[استكشاف الأخطاء الم CA وإصلاحها](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[نهج استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

لحماية البريد الإلكتروني (Exchange Online) من الوصول بواسطة الأجهزة غير المتوافقة، يجب أن يكون المستندان متبوعين بما يلي:

1. [حماية الوصول إلى البريد الإلكتروني من الأجهزة التي تستخدم EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [حماية الوصول إلى البريد الإلكتروني من الأجهزة التي تستخدم عملاء المصادقة الحديثة مثل Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)