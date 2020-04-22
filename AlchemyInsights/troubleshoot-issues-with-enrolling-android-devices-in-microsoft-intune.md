---
title: استكشاف المشاكل المتعلقة بتسجيل أجهزة Android في Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759607"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>استكشاف المشاكل المتعلقة بتسجيل أجهزة Android في Microsoft Intune

راجع الموارد المذكورة أدناه لحل مشكلتك الآن.
  
بعض القضايا الشائعة وخطوات الحل:
  
 **خطأ غير مشفر في الجهاز في بوابة الشركة:** تتطلب الإصدارات الأحدث من Android ، خاصة ً بدءًا من v7.0 ، رمز مرور بدء التشغيل للتأكد من تشفير جهازك بالكامل. الحلول الشائعة هي تمكين دبوس بدء التشغيل أو تشفير الجهاز بالكامل. راجع [هذا المستند](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) لمزيد من المعلومات.
  
 **تفشل الأجهزة في تسجيل الوصول باستخدام خدمة Intune أو عرضها كـ "غير صحية" في وحدة تحكم إدارة Intune:** قد لا تحقق بعض أجهزة سامسونج 4.4 و5.5 في الخدمة. هناك 3 حلول ممكنة لهذه المشكلة:
  
1. افتح تطبيق بوابة شركة Intune يدويًا، والذي سيبدأ مزامنة الجهاز تلقائيًا.

2. تحديث الجهاز إلى الروبوت 6.0 أو أعلى.

3. تعطيل مدير سامسونج الذكي من إدارة بوابة شركة Intune. راجع [هذه الوثيقة](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) لمزيد من التفاصيل حول هذه القضايا والقرارات.

 **خطأ غير صالح** أو اسم المستخدم غير معروف نوع ترخيص **المستخدم:** يحتاج المستخدم إلى تعيين ترخيص Intune أو EMS. راجع هذه المستندات لتعيين ترخيص من خلال: مركز Office Admin أو بوابة Azure.
  
موارد إضافية للمساعدة في حل مشكلتك:
  
1. استخدم [بوابة استكشاف الأخطاء وإصلاحها Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص حالات فشل التسجيل الشائعة وحلها. راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) لمزيد من التفاصيل.

2. راجع [هذا المستند](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) للحصول على قائمة بالأخطاء الشائعة التي تمنع التسجيل والحلول لكل منها.

3. [تعرّف على كيفية تسجيل أجهزة Android في Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
