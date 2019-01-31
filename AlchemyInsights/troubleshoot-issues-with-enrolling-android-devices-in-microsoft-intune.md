---
title: استكشاف مشكلات تسجيل أجهزة الروبوت في Microsoft إينتوني
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655870"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>استكشاف مشكلات تسجيل أجهزة الروبوت في Microsoft إينتوني

مراجعة الموارد المذكورة أدناه لحل المشكلة التي تواجهها الآن.
  
بعض المشاكل الشائعة ودقة الخطوات:
  
 **الجهاز غير مشفرة خطأ في "مدخل الشركة على الإنترنت":** تتطلب الإصدارات الأحدث من الروبوت، بدءاً v7.0، لا سيما رمز مرور بدء تشغيل للتأكد من أن الجهاز مشفرة بالكامل. يتم إيجاد حلول مشتركة لتمكين pin بدء تشغيل أو تشفير الجهاز تماما. مراجعة [هذا المستند](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) للحصول على مزيد من المعلومات. 
  
 **فشل أجهزة للتحقق بخدمة إينتوني أو عرض ك "الصحية" في وحدة تحكم المسؤول إينتوني:** قد لا تحقق بعض 4.4 سامسونج وأجهزة 5.5 إلى الخدمة. هناك 3 الحلول الممكنة لهذه المشكلة: 
  
1. فتح التطبيق "مدخل الشركة إينتوني"، الذي سيبدأ تلقائياً مزامنة جهاز يدوياً.
    
2. تحديث الجهاز إلى 6.0 الروبوت أو أعلى.
    
3. تعطيل "إدارة الذكية سامسونج" من إدارة "مدخل الشركة إينتوني". مراجعة [هذا المستند](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) لمزيد من التفاصيل عن هذه المشاكل والحلول. 
    
 **نوع المستخدم ترخيص غير صالح** أو **"المستخدم يتم التعرف على اسم" الخطأ:** يحتاج المستخدم لتعيين ترخيص إينتوني أو نظم الإدارة البيئية. مراجعة هذه المستندات لتعيين ترخيص إلى: مدخل مركز مسؤول Office أو Azure. 
  
موارد إضافية للمساعدة في حل المشكلة:
  
1. استخدام [إينتوني مدخل استكشاف الأخطاء وإصلاحها](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص وحل فشل التسجيل الشائعة. مراجعة [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول على مزيد من التفاصيل. 
    
2. مراجعة [هذا المستند](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) للحصول على قائمة أخطاء الشائعة التي تمنع التسجيل والحلول لكل. 
    
3. [التعرف على كيفية تسجيل أجهزة الروبوت في Microsoft إينتوني](https://docs.microsoft.com/intune/android-enroll).
    

