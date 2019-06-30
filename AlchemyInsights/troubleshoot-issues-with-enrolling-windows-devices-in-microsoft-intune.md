---
title: استكشاف مشكلات تسجيل أجهزة Windows في Microsoft إينتوني
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: fa48b76fb49cdeef0734e77520c9bf95c150f317
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353524"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>استكشاف مشكلات تسجيل أجهزة Windows في Microsoft إينتوني

مراجعة الموارد المذكورة أدناه لحل المشكلة التي تواجهها الآن.
  
بعض رسائل الخطأ الشائعة ودقة الخطوات:
  
 **لا يمكن تثبيت البرنامج، 0x80cf4017:** انتهت صلاحية شهادة الحساب الخاص بك. إعادة تحميل حزمة برامج الكمبيوتر العميل في وحدة تحكم الإدارة إينتوني. مراجعة هذه الوثائق للحصول على مزيد من المعلومات.
  
 **رمز الخطأ 0x801c0003:** يمكن أن يحدث الخطأ في السيناريوهات التالية:
  
1. ليس لدى المستخدم المزيد من أجهزة تسجيل من حد الجهاز. مراجعة هذه المستندات [إزالة جهاز](https://docs.microsoft.com/intune/devices-wipe) أو [تغيير حد الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

2. يتم تعيين "المستخدمين قد وصل الأجهزة لإعلان Azure" إلى "بلا". تعيين للكل أو تحديد المستخدمين. مراجعة [هذه الوثائق](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) للحصول على مزيد من المعلومات.

3. تم تسجيل الجهاز مسبقاً من قبل مستخدم آخر. إذا كان الأمر كذلك، إزالة الجهاز من وحدة Azure إينتوني أو أونينرول الجهاز يدوياً قبل المحاولة مرة أخرى.

4. الجهاز هو 10 Windows Home. وصل فقط Windows 10 Pro والتعليم ووحدات Sku المؤسسة Azure Active Directory.

موارد إضافية للمساعدة في حل المشكلة:
  
1. استخدام [إينتوني مدخل استكشاف الأخطاء وإصلاحها](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص وحل فشل التسجيل الشائعة. مراجعة [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول على مزيد من التفاصيل.

2. مراجعة هذه الوثائق للحصول على قائمة أخطاء الشائعة التي تمنع التسجيل والحلول لكل: [دليل استكشاف الأخطاء وإصلاحها](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) و [مستند استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[التعرف على كيفية تسجيل أجهزة Windows في Microsoft إينتوني](https://docs.microsoft.com/intune/windows-enroll).
