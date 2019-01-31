---
title: استكشاف مشكلات تسجيل أجهزة دائرة الرقابة الداخلية في Microsoft إينتوني
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: cd1afc83fe98f363aee4c3324a634c200cd08947
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658426"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>استكشاف مشكلات تسجيل أجهزة دائرة الرقابة الداخلية في Microsoft إينتوني

مراجعة الموارد المذكورة أدناه لحل المشكلة التي تواجهها الآن. 
  
بعض رسائل الخطأ الشائعة ودقة الخطوات:
  
- **الوصول إلى الحد الأقصى الجهاز** ليس لدى المستخدم المزيد من أجهزة تسجيل من حد الجهاز. مراجعة هذه المستندات [إزالة جهاز](https://docs.microsoft.com/intune/devices-wipe) أو [تغيير حد الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **"الخدمة هذا" غير معتمد. لا يوجد نهج التسجيل:** أبل دفع إعلام خدمة (أسماء APN) يحتاج إلى تكوين أو تجديدها. مراجعة [هذا المستند](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) للحصول على إرشادات حول كيفية القيام بذلك. 
    
- **صالح نوع ترخيص المستخدم أو اسم المستخدم غير معترف به:** يحتاج المستخدم لتعيين ترخيص إينتوني أو نظم الإدارة البيئية. مراجعة هذه المستندات لتعيين ترخيص إلى: [مركز مسؤول Office](https://docs.microsoft.com/intune/licenses-assign) أو [موقع Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
موارد إضافية للمساعدة في حل المشكلة:
  
1. استخدام [إينتوني مدخل استكشاف الأخطاء وإصلاحها](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص وحل فشل التسجيل الشائعة. مراجعة [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول على مزيد من التفاصيل. 
    
2. مراجعة هذه الوثائق للحصول على قائمة أخطاء الشائعة التي تمنع التسجيل والحلول لكل: [دليل استكشاف الأخطاء وإصلاحها](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) و [مستند استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [التعرف على كيفية تسجيل أجهزة دائرة الرقابة الداخلية في Microsoft إينتوني](https://docs.microsoft.com/intune/ios-enroll).
    

