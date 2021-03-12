---
title: استكشاف المشاكل المتعلقة بتسجيل أجهزة iOS في Microsoft Intune وإصلاحها
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
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708949"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>استكشاف المشاكل المتعلقة بتسجيل أجهزة iOS في Microsoft Intune وإصلاحها

راجع الموارد المدرجة أدناه لحل المشكلة الآن. 
  
بعض رسائل الخطأ الشائعة وبعض خطوات الحل:
  
- **تم الوصول إلى غطاء الجهاز** لدى المستخدم عدد من الأجهزة مسجل أكثر من حد الجهاز. راجع هذه المستندات [لإزالة جهاز](https://docs.microsoft.com/intune/devices-wipe) أو [تغيير حد الجهاز.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **هذه الخدمة غير معتمدة. لا يوجد نهج تسجيل:** يجب تكوين خدمة الإعلامات من Apple (APNS) أو تجديدها. راجع [هذا المستند](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) للحصول على إرشادات حول كيفية القيام بذلك. 
    
- **نوع ترخيص المستخدم غير صالح أو اسم المستخدم غير متعرف عليه:** يجب تعيين ترخيص Intune أو EMS للمستخدم. راجع هذه المستندات لتعيين ترخيص من خلال: [مركز إدارة Office](https://docs.microsoft.com/intune/licenses-assign) أو مدخل [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
موارد إضافية للمساعدة في حل المشكلة:
  
1. استخدم مدخل استكشاف الأخطاء وإصلاحها في [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص حالات الفشل الشائعة في التسجيل وحلها. راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول على مزيد من التفاصيل. 
    
2. راجع هذه المستندات للحصول على قائمة الأخطاء الشائعة التي تمنع التسجيل والقرارات لكل [منها:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) دليل استكشاف الأخطاء وإصلاحها ومستند استكشاف [الأخطاء وإصلاحها.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [تعرف على كيفية تسجيل أجهزة iOS في Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

