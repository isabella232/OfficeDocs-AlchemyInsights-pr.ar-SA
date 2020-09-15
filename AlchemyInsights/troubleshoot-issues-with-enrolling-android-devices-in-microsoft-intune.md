---
title: استكشاف الأخطاء وإصلاحها باستخدام أجهزه Android في Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689941"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>استكشاف الأخطاء وإصلاحها باستخدام أجهزه Android في Microsoft Intune

راجع الموارد المدرجة أدناه لحل المشكلة الآن.
  
بعض المشاكل الشائعة وخطوات الحل:
  
 **خطا غير مشفر في الجهاز في مدخل الشركة:** تتطلب الإصدارات الأحدث من نظام التشغيل Android ، والتي تبدا ب v 7.0 ، رمز مرور بدء التشغيل للتاكد من ان جهازك مشفر بالبالكامل. الحلول الشائعة هي تمكين رمز pin لبدء التشغيل أو تشفير الجهاز بالبالكامل. راجع [هذا المستند](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) للحصول علي مزيد من المعلومات.
  
 **فشلت الاجهزه في إيداع الخدمة أو عرضها ك "غير سليم" في وحده تحكم مسؤول Intune:** قد لا تتحقق بعض أجهزه Samsung 4.4 و 5.5 من الخدمة. هناك 3 حلول محتمله لهذه المشكلة:
  
1. افتح تطبيق Intune company Portal يدويا ، مما يؤدي إلى بدء مزامنة جهاز تلقائيا.

2. تحديث الجهاز إلى Android 6.0 أو إصدار أحدث.

3. تعطيل Samsung الاداره الذكية من أداره مدخل شركه Intune. راجع [هذا المستند](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) للحصول علي مزيد من التفاصيل حول هذه المشاكل والحلول.

 **نوع ترخيص المستخدم غير صالح** أو **غير معروف اسم المستخدم:** يجب ان يتم تعيين ترخيص Intune أو EMS إلى المستخدم. راجع هذه المستندات لتعيين ترخيص عبر: مركز أداره Office أو مدخل Azure.
  
موارد اضافيه للمساعدة في حل المشكلة:
  
1. استخدام [مدخل Intune استكشاف الأخطاء وإصلاحها](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص فشل التسجيل الشائع وتصحيحه. راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول علي مزيد من التفاصيل.

2. راجع [هذا المستند](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) للحصول علي قائمه بالأخطاء الشائعة التي تمنع التسجيل والحلول لكل منها.

3. [تعرف علي كيفيه تسجيل أجهزه Android في Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
