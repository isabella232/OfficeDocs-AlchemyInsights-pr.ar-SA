---
title: استكشاف المشاكل المتعلقة بتسجيل أجهزة Windows في Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665819"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>استكشاف المشاكل المتعلقة بتسجيل أجهزة Windows في Microsoft Intune

راجع الموارد المذكورة أدناه لحل مشكلتك الآن.
  
بعض رسائل الخطأ الشائعة وخطوات الدقة:
  
 **لا يمكن تثبيت البرنامج، 0x80cf4017:** انتهت صلاحية شهادة حسابك. إعادة تحميل حزمة برامج عميل الكمبيوتر في وحدة تحكم الإدارة Intune. راجع هذه الوثائق لمزيد من المعلومات.
  
 **رمز الخطأ 0x801c0003:** يمكن أن يحدث الخطأ في السيناريوهات التالية:
  
-  لدى المستخدم أجهزة أكثر تسجيلًا من حد الجهاز. راجع هذه المستندات [لإزالة جهاز](https://docs.microsoft.com/intune/devices-wipe) أو تغيير [حد الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "قد ينضم المستخدمون إلى الأجهزة إلى Azure AD" تم تعيينه إلى "لا شيء". قم بتعيينها إلى كافة المستخدمين أو حددها. راجع [هذه الوثائق](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) لمزيد من المعلومات.

-  تم تسجيل الجهاز بالفعل من قبل مستخدم آخر. إذا كان الأمر كذلك، قم بإزالة الجهاز من وحدة تحكم Azure Intune أو قم بإلغاء تسجيل الجهاز يدويًا قبل المحاولة مرة أخرى.

-  الجهاز هو ويندوز 10 الرئيسية. يمكن فقط لـ Windows 10 Pro والتعليم والشركات الصغيرة والمتوسطة الانضمام إلى Azure Active Directory.

موارد إضافية للمساعدة في حل مشكلتك:
  
-  استخدم [بوابة استكشاف الأخطاء وإصلاحها Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص حالات فشل التسجيل الشائعة وحلها. راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) لمزيد من التفاصيل.

-  راجع هذه المستندات للحصول على قائمة من الأخطاء الشائعة التي تمنع التسجيل والحلول لكل: [دليل استكشاف الأخطاء وإصلاحها](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) [ومستند استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[تعرّف على كيفية تسجيل أجهزة Windows في Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
