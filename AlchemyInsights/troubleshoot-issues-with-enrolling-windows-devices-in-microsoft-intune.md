---
title: استكشاف الأخطاء وإصلاحها في تسجيل أجهزه Windows في Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658865"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>استكشاف الأخطاء وإصلاحها في تسجيل أجهزه Windows في Microsoft Intune

راجع الموارد المدرجة أدناه لحل المشكلة الآن.
  
بعض رسائل الخطا الشائعة وخطوات الدقة:
  
 **لا يمكن تثبيت البرنامج ، 0x80cf4017:** انتهت صلاحيه شهادة حسابك. قم باعاده تنزيل حزمه برامج عميل الكمبيوتر الشخصي في وحده تحكم مسؤول Intune. راجع هذه الوثائق للحصول علي مزيد من المعلومات.
  
 **رمز الخطا 0x801c0003:** يمكن ان يحدث الخطا في السيناريوهات التالية:
  
-  يملك المستخدم المزيد من الاجهزه التي تم تسجيلها من حد الجهاز. راجع هذه المستندات [لأزاله جهاز](https://docs.microsoft.com/intune/devices-wipe) أو [تغيير حد الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "يمكن ان ينضم المستخدمون إلى الاجهزه التي تم تعيينها إلى" بلا ". قم بتعيينه إلى جميع المستخدمين أو حددهم. راجع [هذه الوثائق](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) للحصول علي مزيد من المعلومات.

-  تم تسجيل الجهاز بالفعل من قبل مستخدم آخر. إذا كانت هذه هي الحالة ، فقم بازاله الجهاز من وحده التحكم Azure Intune أو أونينرول الجهاز يدويا قبل المحاولة مره أخرى.

-  الجهاز هو Windows 10 Home. يمكن لنظام التشغيل Windows 10 Pro والتعليم ووحدات Sku للمؤسسة الانضمام إلى Azure Active directory.

موارد اضافيه للمساعدة في حل المشكلة:
  
-  استخدام [مدخل Intune استكشاف الأخطاء وإصلاحها](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص فشل التسجيل الشائع وتصحيحه. راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول علي مزيد من التفاصيل.

-  راجع المستندات التالية للحصول علي قائمه بالأخطاء الشائعة التي تمنع التسجيل والحلول لكل منها: [دليل استكشاف الأخطاء](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) وإصلاحها [واستكشاف أخطاء المستند](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[تعرف علي كيفيه تسجيل أجهزه Windows في Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
