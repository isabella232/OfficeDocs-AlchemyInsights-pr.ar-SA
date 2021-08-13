---
title: استكشاف المشاكل المتعلقة بتسجيل أجهزة Android في الأجهزة التي تعمل بنظام التشغيل Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008065"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>استكشاف المشاكل المتعلقة بتسجيل أجهزة Android في الأجهزة التي تعمل بنظام التشغيل Microsoft Intune

راجع الموارد المدرجة أدناه لحل المشكلة الآن.
  
بعض المشاكل الشائعة والخطوات المتعلقة بال حل:
  
 **خطأ "الجهاز غير مشفر" في Company Portal:** تتطلب الإصدارات الأحدث من Android، خاصة بدءا من الإصدار 7.0، رمز دخول بدء التشغيل للتأكد من أن جهازك مشفر بالكامل. الحلول الشائعة هي تمكين دبوس بدء التشغيل أو تشفير الجهاز بالكامل. راجع [هذا المستند](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) للحصول على مزيد من المعلومات.
  
 تفشل الأجهزة في تسجيل الدخول باستخدام خدمة Intune أو عرضها ك **"غير صحية" في وحدة تحكم مسؤول Intune:** قد لا تدقق بعض أجهزة Samsung 4.4 و5.5 في الخدمة. هناك 3 حلول محتملة لهذه المشكلة:
  
1. افتح تطبيق Intune Company Portal يدويا، مما يؤدي إلى بدء مزامنة الجهاز تلقائيا.

2. تحديث الجهاز إلى Android 6.0 أو إصدار أحدث.

3. قم بتعطيل Samsung Smart Manager من إدارة Intune Company Portal. راجع [هذا المستند](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) للحصول على مزيد من التفاصيل حول هذه المشاكل والقرارات.

 **خطأ نوع ترخيص المستخدم غير صالح** أو اسم المستخدم غير متعرف **عليه:** يجب تعيين ترخيص Intune أو EMS للمستخدم. راجع هذه المستندات لتعيين ترخيص من خلال: Office مركز الإدارة أو مدخل Azure.
  
موارد إضافية للمساعدة في حل المشكلة:
  
1. استخدم مدخل استكشاف الأخطاء وإصلاحها في [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص حالات فشل التسجيل الشائعة وحلها. راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول على مزيد من التفاصيل.

2. راجع [هذا المستند](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) للحصول على قائمة الأخطاء الشائعة التي تمنع التسجيل والقرارات لكل منها.

3. [تعرف على كيفية تسجيل أجهزة Android في Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
