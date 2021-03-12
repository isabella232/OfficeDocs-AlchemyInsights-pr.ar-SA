---
title: استكشاف المشاكل المتعلقة بتسجيل أجهزة iOS في Microsoft Intune وإصلاحها
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
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708949"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="24adc-102">استكشاف المشاكل المتعلقة بتسجيل أجهزة iOS في Microsoft Intune وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="24adc-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="24adc-103">راجع الموارد المدرجة أدناه لحل المشكلة الآن.</span><span class="sxs-lookup"><span data-stu-id="24adc-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="24adc-104">بعض رسائل الخطأ الشائعة وبعض خطوات الحل:</span><span class="sxs-lookup"><span data-stu-id="24adc-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="24adc-105">**تم الوصول إلى غطاء الجهاز** لدى المستخدم عدد من الأجهزة مسجل أكثر من حد الجهاز.</span><span class="sxs-lookup"><span data-stu-id="24adc-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="24adc-106">راجع هذه المستندات [لإزالة جهاز](https://docs.microsoft.com/intune/devices-wipe) أو [تغيير حد الجهاز.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="24adc-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="24adc-107">**هذه الخدمة غير معتمدة. لا يوجد نهج تسجيل:** يجب تكوين خدمة الإعلامات من Apple (APNS) أو تجديدها.</span><span class="sxs-lookup"><span data-stu-id="24adc-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="24adc-108">راجع [هذا المستند](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) للحصول على إرشادات حول كيفية القيام بذلك.</span><span class="sxs-lookup"><span data-stu-id="24adc-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="24adc-109">**نوع ترخيص المستخدم غير صالح أو اسم المستخدم غير متعرف عليه:** يجب تعيين ترخيص Intune أو EMS للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="24adc-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="24adc-110">راجع هذه المستندات لتعيين ترخيص من خلال: [مركز إدارة Office](https://docs.microsoft.com/intune/licenses-assign) أو مدخل [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="24adc-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="24adc-111">موارد إضافية للمساعدة في حل المشكلة:</span><span class="sxs-lookup"><span data-stu-id="24adc-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="24adc-112">استخدم مدخل استكشاف الأخطاء وإصلاحها في [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص حالات الفشل الشائعة في التسجيل وحلها.</span><span class="sxs-lookup"><span data-stu-id="24adc-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="24adc-113">راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول على مزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="24adc-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="24adc-114">راجع هذه المستندات للحصول على قائمة الأخطاء الشائعة التي تمنع التسجيل والقرارات لكل [منها:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) دليل استكشاف الأخطاء وإصلاحها ومستند استكشاف [الأخطاء وإصلاحها.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="24adc-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="24adc-115">[تعرف على كيفية تسجيل أجهزة iOS في Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="24adc-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

