---
title: استكشاف المشاكل المتعلقة بتسجيل أجهزة iOS في Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736145"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>استكشاف المشاكل المتعلقة بتسجيل أجهزة iOS في Microsoft Intune

راجع الموارد المذكورة أدناه لحل مشكلتك الآن. 
  
بعض رسائل الخطأ الشائعة وخطوات الدقة:
  
- **تم الوصول إلى غطاء الجهاز** لدى المستخدم أجهزة أكثر تسجيلًا من حد الجهاز. راجع هذه المستندات [لإزالة جهاز](https://docs.microsoft.com/intune/devices-wipe) أو تغيير [حد الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **هذه الخدمة غير معتمدة. لا توجد سياسة تسجيل:** يجب تكوين خدمة إعلام Apple Push (APNS) أو تجديدها. راجع [هذا المستند](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) للحصول على إرشادات حول كيفية القيام بذلك. 
    
- **نوع ترخيص المستخدم غير صالح أو اسم المستخدم غير معترف به:** يجب أن يتم تعيين ترخيص Intune أو EMS للمستخدم. راجع هذه المستندات لتعيين ترخيص من خلال: [مركز Office Admin](https://docs.microsoft.com/intune/licenses-assign) أو بوابة [Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
موارد إضافية للمساعدة في حل مشكلتك:
  
1. استخدم [بوابة استكشاف الأخطاء وإصلاحها Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص حالات فشل التسجيل الشائعة وحلها. راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) لمزيد من التفاصيل. 
    
2. راجع هذه المستندات للحصول على قائمة من الأخطاء الشائعة التي تمنع التسجيل والحلول لكل: [دليل استكشاف الأخطاء وإصلاحها](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) [ومستند استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [تعرّف على كيفية تسجيل أجهزة iOS في Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

