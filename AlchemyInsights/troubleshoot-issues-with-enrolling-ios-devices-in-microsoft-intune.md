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
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="d1b53-102">استكشاف مشكلات تسجيل أجهزة دائرة الرقابة الداخلية في Microsoft إينتوني</span><span class="sxs-lookup"><span data-stu-id="d1b53-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="d1b53-103">مراجعة الموارد المذكورة أدناه لحل المشكلة التي تواجهها الآن.</span><span class="sxs-lookup"><span data-stu-id="d1b53-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="d1b53-104">بعض رسائل الخطأ الشائعة ودقة الخطوات:</span><span class="sxs-lookup"><span data-stu-id="d1b53-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="d1b53-p101">**الوصول إلى الحد الأقصى الجهاز** ليس لدى المستخدم المزيد من أجهزة تسجيل من حد الجهاز. مراجعة هذه المستندات [إزالة جهاز](https://docs.microsoft.com/intune/devices-wipe) أو [تغيير حد الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="d1b53-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="d1b53-p102">**"الخدمة هذا" غير معتمد. لا يوجد نهج التسجيل:** أبل دفع إعلام خدمة (أسماء APN) يحتاج إلى تكوين أو تجديدها. مراجعة [هذا المستند](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) للحصول على إرشادات حول كيفية القيام بذلك.</span><span class="sxs-lookup"><span data-stu-id="d1b53-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="d1b53-p103">**صالح نوع ترخيص المستخدم أو اسم المستخدم غير معترف به:** يحتاج المستخدم لتعيين ترخيص إينتوني أو نظم الإدارة البيئية. مراجعة هذه المستندات لتعيين ترخيص إلى: [مركز مسؤول Office](https://docs.microsoft.com/intune/licenses-assign) أو [موقع Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="d1b53-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="d1b53-111">موارد إضافية للمساعدة في حل المشكلة:</span><span class="sxs-lookup"><span data-stu-id="d1b53-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d1b53-p104">استخدام [إينتوني مدخل استكشاف الأخطاء وإصلاحها](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص وحل فشل التسجيل الشائعة. مراجعة [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول على مزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="d1b53-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="d1b53-114">مراجعة هذه الوثائق للحصول على قائمة أخطاء الشائعة التي تمنع التسجيل والحلول لكل: [دليل استكشاف الأخطاء وإصلاحها](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) و [مستند استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="d1b53-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="d1b53-115">[التعرف على كيفية تسجيل أجهزة دائرة الرقابة الداخلية في Microsoft إينتوني](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="d1b53-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

