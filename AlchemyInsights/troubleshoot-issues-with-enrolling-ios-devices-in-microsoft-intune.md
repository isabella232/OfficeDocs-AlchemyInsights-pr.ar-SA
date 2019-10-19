---
title: استكشاف مشكلات تسجيل أجهزه iOS في Microsoft اينتوني وإصلاحها
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36506864"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>استكشاف مشكلات تسجيل أجهزه iOS في Microsoft اينتوني وإصلاحها

راجع الموارد المذكورة أدناه لحل مشكلتك الآن. 
  
بعض رسائل الخطا الشائعة وخطوات الدقة:
  
- **تم الوصول إلى غطاء الجهاز** لدي المستخدم المزيد من الاجهزه المسجلة من حد الجهاز. راجع هذه المستندات [لأزاله جهاز](https://docs.microsoft.com/intune/devices-wipe) أو [تغيير حد الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **هذه الخدمة غير معتمده. لا توجد سياسة انتساب:** يجب ان يتم تكوين أو تجديد خدمه الاعلام الدفع من Apple (APNS). راجع [هذا المستند](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) للحصول علي إرشادات حول كيفيه القيام بذلك. 
    
- **نوع ترخيص المستخدم غير صالح أو لم يتم التعرف علي اسم المستخدم:** يحتاج المستخدم إلى تعيين اينتوني أو ترخيص EMS. مراجعه هذه المستندات لتعيين ترخيص من خلال: [مركز مسؤول Office](https://docs.microsoft.com/intune/licenses-assign) أو [المدخل الأزرق السماوي](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
موارد اضافيه للمساعدة في حل مشكلتك:
  
1. استخدام [بوابه استكشاف الأخطاء وإصلاحها اينتوني](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص وحل فشل التسجيل الشائعة. راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول علي مزيد من التفاصيل. 
    
2. راجع هذه المستندات للحصول علي قائمه بالأخطاء الشائعة التي تمنع التسجيل والدقة لكل منها: [دليل استكشاف](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) الأخطاء وإصلاحها وحل [المشاكل](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [تعرف علي كيفيه تسجيل أجهزه iOS في Microsoft اينتوني](https://docs.microsoft.com/intune/ios-enroll).
    

