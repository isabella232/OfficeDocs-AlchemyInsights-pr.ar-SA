---
title: استكشاف مشكلات تسجيل أجهزة Windows في Microsoft إينتوني
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28273808"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="bb54e-102">استكشاف مشكلات تسجيل أجهزة Windows في Microsoft إينتوني</span><span class="sxs-lookup"><span data-stu-id="bb54e-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="bb54e-103">مراجعة الموارد المذكورة أدناه لحل المشكلة التي تواجهها الآن.</span><span class="sxs-lookup"><span data-stu-id="bb54e-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="bb54e-104">بعض رسائل الخطأ الشائعة ودقة الخطوات:</span><span class="sxs-lookup"><span data-stu-id="bb54e-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="bb54e-p101">**لا يمكن تثبيت البرنامج، 0x80cf4017:** انتهت صلاحية شهادة الحساب الخاص بك. إعادة تحميل حزمة برامج الكمبيوتر العميل في وحدة تحكم الإدارة إينتوني. مراجعة هذه الوثائق للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="bb54e-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="bb54e-108">**رمز الخطأ 0x801c0003:** يمكن أن يحدث الخطأ في السيناريوهات التالية:</span><span class="sxs-lookup"><span data-stu-id="bb54e-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="bb54e-p102">ليس لدى المستخدم المزيد من أجهزة تسجيل من حد الجهاز. مراجعة هذه المستندات [إزالة جهاز](https://docs.microsoft.com/en-us/intune/devices-wipe) أو [تغيير حد الجهاز](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="bb54e-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="bb54e-p103">يتم تعيين "المستخدمين قد وصل الأجهزة لإعلان Azure" إلى "بلا". تعيين للكل أو تحديد المستخدمين. مراجعة [هذه الوثائق](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="bb54e-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="bb54e-p104">تم تسجيل الجهاز مسبقاً من قبل مستخدم آخر. إذا كان الأمر كذلك، إزالة الجهاز من وحدة Azure إينتوني أو أونينرول الجهاز يدوياً قبل المحاولة مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="bb54e-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="bb54e-p105">الجهاز هو 10 Windows Home. وصل فقط Windows 10 Pro والتعليم ووحدات Sku المؤسسة Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bb54e-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="bb54e-118">موارد إضافية للمساعدة في حل المشكلة:</span><span class="sxs-lookup"><span data-stu-id="bb54e-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="bb54e-p106">استخدام [إينتوني مدخل استكشاف الأخطاء وإصلاحها](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص وحل فشل التسجيل الشائعة. مراجعة [هذا المستند](https://docs.microsoft.com/en-us/intune/help-desk-operators) للحصول على مزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="bb54e-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="bb54e-121">مراجعة هذه الوثائق للحصول على قائمة أخطاء الشائعة التي تمنع التسجيل والحلول لكل: [دليل استكشاف الأخطاء وإصلاحها](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) و [مستند استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="bb54e-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="bb54e-122">[التعرف على كيفية تسجيل أجهزة Windows في Microsoft إينتوني](https://docs.microsoft.com/en-us/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="bb54e-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span></span>
  

