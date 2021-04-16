---
title: استكشاف المشاكل المتعلقة بتسجيل أجهزة Windows في Microsoft Intune وإصلاحها
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808958"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>استكشاف المشاكل المتعلقة بتسجيل أجهزة Windows في Microsoft Intune وإصلاحها

راجع الموارد المدرجة أدناه لحل المشكلة الآن.
  
بعض رسائل الخطأ الشائعة والخطوات اللازمة لحلها:
  
 **لا يمكن تثبيت البرنامج، 0x80cf4017:** انتهت صلاحية شهادة حسابك. إعادة تنزيل حزمة برامج عميل الكمبيوتر الشخصي في وحدة تحكم مسؤول Intune. راجع هذه الوثائق للحصول على مزيد من المعلومات.
  
 **رمز الخطأ 0x801c0003:** يمكن أن يحدث الخطأ في السيناريوهات التالية:
  
-  لدى المستخدم عدد أجهزة مسجل أكثر من حد الجهاز. راجع هذه المستندات [لإزالة جهاز أو](https://docs.microsoft.com/intune/devices-wipe) تغيير حد [الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  يتم تعيين "قد يقوم المستخدمون بضم الأجهزة إلى Azure AD" إلى "بلا". قم بتعيينه إلى جميع المستخدمين أو حدده. راجع [هذه الوثائق](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) للحصول على مزيد من المعلومات.

-  تم تسجيل الجهاز بالفعل من قبل مستخدم آخر. إذا كان الأمر كذلك، فإزالة الجهاز من وحدة تحكم Azure Intune أو إلغاء تشغيل الجهاز يدويا قبل المحاولة مرة أخرى.

-  الجهاز هو Windows 10 Home. يمكن فقط ل Windows 10 Pro و Education و Enterprise SKUs الانضمام إلى Azure Active Directory.

موارد إضافية للمساعدة في حل المشكلة:
  
-  استخدم مدخل استكشاف الأخطاء وإصلاحها في [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص حالات فشل التسجيل الشائعة وحلها. راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول على مزيد من التفاصيل.

-  راجع هذه المستندات للحصول على قائمة الأخطاء الشائعة التي تمنع التسجيل والقرارات لكل [منها:](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) دليل استكشاف الأخطاء وإصلاحها ومستند [استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[تعرف على كيفية تسجيل أجهزة Windows في Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
