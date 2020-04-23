---
title: استكشاف المشاكل المتعلقة بتسجيل أجهزة iOS في Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736145"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="f3bfd-102">استكشاف المشاكل المتعلقة بتسجيل أجهزة iOS في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f3bfd-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="f3bfd-103">راجع الموارد المذكورة أدناه لحل مشكلتك الآن.</span><span class="sxs-lookup"><span data-stu-id="f3bfd-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="f3bfd-104">بعض رسائل الخطأ الشائعة وخطوات الدقة:</span><span class="sxs-lookup"><span data-stu-id="f3bfd-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="f3bfd-105">**تم الوصول إلى غطاء الجهاز** لدى المستخدم أجهزة أكثر تسجيلًا من حد الجهاز.</span><span class="sxs-lookup"><span data-stu-id="f3bfd-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="f3bfd-106">راجع هذه المستندات [لإزالة جهاز](https://docs.microsoft.com/intune/devices-wipe) أو تغيير [حد الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="f3bfd-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="f3bfd-107">**هذه الخدمة غير معتمدة. لا توجد سياسة تسجيل:** يجب تكوين خدمة إعلام Apple Push (APNS) أو تجديدها.</span><span class="sxs-lookup"><span data-stu-id="f3bfd-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="f3bfd-108">راجع [هذا المستند](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) للحصول على إرشادات حول كيفية القيام بذلك.</span><span class="sxs-lookup"><span data-stu-id="f3bfd-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="f3bfd-109">**نوع ترخيص المستخدم غير صالح أو اسم المستخدم غير معترف به:** يجب أن يتم تعيين ترخيص Intune أو EMS للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="f3bfd-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="f3bfd-110">راجع هذه المستندات لتعيين ترخيص من خلال: [مركز Office Admin](https://docs.microsoft.com/intune/licenses-assign) أو بوابة [Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="f3bfd-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="f3bfd-111">موارد إضافية للمساعدة في حل مشكلتك:</span><span class="sxs-lookup"><span data-stu-id="f3bfd-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="f3bfd-112">استخدم [بوابة استكشاف الأخطاء وإصلاحها Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص حالات فشل التسجيل الشائعة وحلها.</span><span class="sxs-lookup"><span data-stu-id="f3bfd-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="f3bfd-113">راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) لمزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="f3bfd-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="f3bfd-114">راجع هذه المستندات للحصول على قائمة من الأخطاء الشائعة التي تمنع التسجيل والحلول لكل: [دليل استكشاف الأخطاء وإصلاحها](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) [ومستند استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="f3bfd-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="f3bfd-115">[تعرّف على كيفية تسجيل أجهزة iOS في Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="f3bfd-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

