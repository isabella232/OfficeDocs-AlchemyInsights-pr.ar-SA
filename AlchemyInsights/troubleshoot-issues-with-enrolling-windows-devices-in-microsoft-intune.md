---
title: استكشاف مشكلات تسجيل أجهزة Windows في Microsoft إينتوني
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
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665819"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>استكشاف مشكلات تسجيل أجهزة Windows في Microsoft إينتوني

مراجعة الموارد المذكورة أدناه لحل المشكلة التي تواجهها الآن.
  
بعض رسائل الخطأ الشائعة ودقة الخطوات:
  
 **لا يمكن تثبيت البرنامج، 0x80cf4017:** انتهت صلاحية شهادة الحساب الخاص بك. إعادة تحميل حزمة برامج الكمبيوتر العميل في وحدة تحكم الإدارة إينتوني. مراجعة هذه الوثائق للحصول على مزيد من المعلومات.
  
 **رمز الخطأ 0x801c0003:** يمكن أن يحدث الخطأ في السيناريوهات التالية:
  
-  ليس لدى المستخدم المزيد من أجهزة تسجيل من حد الجهاز. مراجعة هذه المستندات [إزالة جهاز](https://docs.microsoft.com/intune/devices-wipe) أو [تغيير حد الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "المستخدمين قد وصل الأجهزة لإعلان Azure" تعيين إلى "بلا". تعيين للكل أو تحديد المستخدمين. مراجعة [هذه الوثائق](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) للحصول على مزيد من المعلومات.

-  تم تسجيل الجهاز مسبقاً من قبل مستخدم آخر. إذا كان الأمر كذلك، إزالة الجهاز من وحدة Azure إينتوني أو أونينرول الجهاز يدوياً قبل المحاولة مرة أخرى.

-  الجهاز هو 10 Windows Home. وصل فقط Windows 10 Pro والتعليم ووحدات Sku المؤسسة Azure Active Directory.

موارد إضافية للمساعدة في حل المشكلة:
  
-  استخدام [إينتوني مدخل استكشاف الأخطاء وإصلاحها](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص وحل فشل التسجيل الشائعة. مراجعة [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول على مزيد من التفاصيل.

-  مراجعة هذه الوثائق للحصول على قائمة أخطاء الشائعة التي تمنع التسجيل والحلول لكل: [دليل استكشاف الأخطاء وإصلاحها](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) و [مستند استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[التعرف على كيفية تسجيل أجهزة Windows في Microsoft إينتوني](https://docs.microsoft.com/intune/windows-enroll).
