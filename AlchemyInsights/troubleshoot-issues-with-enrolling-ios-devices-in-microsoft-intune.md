---
title: استكشاف مشكلات تسجيل أجهزه iOS في Microsoft اينتوني وإصلاحها
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36506864"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="79dc6-102">استكشاف مشكلات تسجيل أجهزه iOS في Microsoft اينتوني وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="79dc6-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="79dc6-103">راجع الموارد المذكورة أدناه لحل مشكلتك الآن.</span><span class="sxs-lookup"><span data-stu-id="79dc6-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="79dc6-104">بعض رسائل الخطا الشائعة وخطوات الدقة:</span><span class="sxs-lookup"><span data-stu-id="79dc6-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="79dc6-105">**تم الوصول إلى غطاء الجهاز** لدي المستخدم المزيد من الاجهزه المسجلة من حد الجهاز.</span><span class="sxs-lookup"><span data-stu-id="79dc6-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="79dc6-106">راجع هذه المستندات [لأزاله جهاز](https://docs.microsoft.com/intune/devices-wipe) أو [تغيير حد الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="79dc6-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="79dc6-107">**هذه الخدمة غير معتمده. لا توجد سياسة انتساب:** يجب ان يتم تكوين أو تجديد خدمه الاعلام الدفع من Apple (APNS).</span><span class="sxs-lookup"><span data-stu-id="79dc6-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="79dc6-108">راجع [هذا المستند](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) للحصول علي إرشادات حول كيفيه القيام بذلك.</span><span class="sxs-lookup"><span data-stu-id="79dc6-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="79dc6-109">**نوع ترخيص المستخدم غير صالح أو لم يتم التعرف علي اسم المستخدم:** يحتاج المستخدم إلى تعيين اينتوني أو ترخيص EMS.</span><span class="sxs-lookup"><span data-stu-id="79dc6-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="79dc6-110">مراجعه هذه المستندات لتعيين ترخيص من خلال: [مركز مسؤول Office](https://docs.microsoft.com/intune/licenses-assign) أو [المدخل الأزرق السماوي](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="79dc6-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="79dc6-111">موارد اضافيه للمساعدة في حل مشكلتك:</span><span class="sxs-lookup"><span data-stu-id="79dc6-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="79dc6-112">استخدام [بوابه استكشاف الأخطاء وإصلاحها اينتوني](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص وحل فشل التسجيل الشائعة.</span><span class="sxs-lookup"><span data-stu-id="79dc6-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="79dc6-113">راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول علي مزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="79dc6-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="79dc6-114">راجع هذه المستندات للحصول علي قائمه بالأخطاء الشائعة التي تمنع التسجيل والدقة لكل منها: [دليل استكشاف](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) الأخطاء وإصلاحها وحل [المشاكل](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="79dc6-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="79dc6-115">[تعرف علي كيفيه تسجيل أجهزه iOS في Microsoft اينتوني](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="79dc6-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

