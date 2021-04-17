---
title: استكشاف المشاكل المتعلقة بتسجيل أجهزة iOS في Microsoft Intune وإصلاحها
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823450"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>استكشاف المشاكل المتعلقة بتسجيل أجهزة iOS في Microsoft Intune وإصلاحها

راجع الموارد المدرجة أدناه لحل المشكلة الآن. 
  
بعض رسائل الخطأ الشائعة والخطوات اللازمة لحلها:
  
- **تم الوصول إلى Cap Device** لدى المستخدم عدد أجهزة مسجل أكثر من حد الجهاز. راجع هذه المستندات [لإزالة جهاز أو](https://docs.microsoft.com/intune/devices-wipe) تغيير حد [الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **هذه الخدمة غير معتمدة. نهج عدم التسجيل:** يجب تكوين خدمة الإعلامات من Apple (APNS) أو تجديدها. راجع [هذا المستند](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) للحصول على إرشادات حول كيفية القيام بذلك. 
    
- **نوع ترخيص المستخدم غير صالح أو اسم المستخدم غير متعرف عليه:** يجب تعيين ترخيص Intune أو EMS للمستخدم. راجع هذه المستندات لتعيين ترخيص من خلال: [مركز إدارة Office](https://docs.microsoft.com/intune/licenses-assign) أو مدخل [Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
موارد إضافية للمساعدة في حل المشكلة:
  
1. استخدم مدخل استكشاف الأخطاء وإصلاحها في [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص حالات فشل التسجيل الشائعة وحلها. راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول على مزيد من التفاصيل. 
    
2. راجع هذه المستندات للحصول على قائمة الأخطاء الشائعة التي تمنع التسجيل والقرارات لكل [منها:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) دليل استكشاف الأخطاء وإصلاحها ومستند [استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [تعرف على كيفية تسجيل أجهزة iOS في Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

