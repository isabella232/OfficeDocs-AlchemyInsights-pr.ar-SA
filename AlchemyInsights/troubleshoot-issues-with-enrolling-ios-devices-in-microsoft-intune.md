---
title: استكشاف المشاكل المتعلقة بتسجيل أجهزه iOS وإصلاحها في Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669235"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="62854-102">استكشاف المشاكل المتعلقة بتسجيل أجهزه iOS وإصلاحها في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="62854-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="62854-103">راجع الموارد المدرجة أدناه لحل المشكلة الآن.</span><span class="sxs-lookup"><span data-stu-id="62854-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="62854-104">بعض رسائل الخطا الشائعة وخطوات الدقة:</span><span class="sxs-lookup"><span data-stu-id="62854-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="62854-105">**الوصول إلى غطاء الجهاز** يملك المستخدم المزيد من الاجهزه التي تم تسجيلها من حد الجهاز.</span><span class="sxs-lookup"><span data-stu-id="62854-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="62854-106">راجع هذه المستندات [لأزاله جهاز](https://docs.microsoft.com/intune/devices-wipe) أو [تغيير حد الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="62854-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="62854-107">**هذه الخدمة غير معتمده. لا يوجد نهج تسجيل:** يجب تكوين خدمه الاعلامات المؤقتة ل Apple (APNS) أو تجديدها.</span><span class="sxs-lookup"><span data-stu-id="62854-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="62854-108">راجع [هذا المستند](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) للحصول علي إرشادات حول كيفيه القيام بذلك.</span><span class="sxs-lookup"><span data-stu-id="62854-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="62854-109">**نوع ترخيص المستخدم غير صالح أو لم يتم التعرف علي اسم المستخدم:** يجب ان يتم تعيين ترخيص Intune أو EMS للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="62854-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="62854-110">راجع هذه المستندات لتعيين ترخيص عبر: [مركز أداره Office](https://docs.microsoft.com/intune/licenses-assign) أو [مدخل Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="62854-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="62854-111">موارد اضافيه للمساعدة في حل المشكلة:</span><span class="sxs-lookup"><span data-stu-id="62854-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="62854-112">استخدام [مدخل Intune استكشاف الأخطاء وإصلاحها](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص فشل التسجيل الشائع وتصحيحه.</span><span class="sxs-lookup"><span data-stu-id="62854-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="62854-113">راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول علي مزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="62854-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="62854-114">راجع المستندات التالية للحصول علي قائمه بالأخطاء الشائعة التي تمنع التسجيل والحلول لكل منها: [دليل استكشاف الأخطاء](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) وإصلاحها [واستكشاف أخطاء المستند](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="62854-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="62854-115">[تعرف علي كيفيه تسجيل أجهزه iOS في Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="62854-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

