---
title: استكشاف المشاكل المتعلقة بتسجيل أجهزه iOS وإصلاحها في Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669235"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>استكشاف المشاكل المتعلقة بتسجيل أجهزه iOS وإصلاحها في Microsoft Intune

راجع الموارد المدرجة أدناه لحل المشكلة الآن. 
  
بعض رسائل الخطا الشائعة وخطوات الدقة:
  
- **الوصول إلى غطاء الجهاز** يملك المستخدم المزيد من الاجهزه التي تم تسجيلها من حد الجهاز. راجع هذه المستندات [لأزاله جهاز](https://docs.microsoft.com/intune/devices-wipe) أو [تغيير حد الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **هذه الخدمة غير معتمده. لا يوجد نهج تسجيل:** يجب تكوين خدمه الاعلامات المؤقتة ل Apple (APNS) أو تجديدها. راجع [هذا المستند](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) للحصول علي إرشادات حول كيفيه القيام بذلك. 
    
- **نوع ترخيص المستخدم غير صالح أو لم يتم التعرف علي اسم المستخدم:** يجب ان يتم تعيين ترخيص Intune أو EMS للمستخدم. راجع هذه المستندات لتعيين ترخيص عبر: [مركز أداره Office](https://docs.microsoft.com/intune/licenses-assign) أو [مدخل Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
موارد اضافيه للمساعدة في حل المشكلة:
  
1. استخدام [مدخل Intune استكشاف الأخطاء وإصلاحها](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص فشل التسجيل الشائع وتصحيحه. راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول علي مزيد من التفاصيل. 
    
2. راجع المستندات التالية للحصول علي قائمه بالأخطاء الشائعة التي تمنع التسجيل والحلول لكل منها: [دليل استكشاف الأخطاء](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) وإصلاحها [واستكشاف أخطاء المستند](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [تعرف علي كيفيه تسجيل أجهزه iOS في Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

