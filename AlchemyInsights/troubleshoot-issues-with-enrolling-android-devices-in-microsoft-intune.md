---
title: استكشاف مشكلات تسجيل أجهزة الروبوت في Microsoft إينتوني
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 9cdfda0d7dd45af260f46738cbc85aac46f53960
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35367276"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="f5839-102">استكشاف مشكلات تسجيل أجهزة الروبوت في Microsoft إينتوني</span><span class="sxs-lookup"><span data-stu-id="f5839-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="f5839-103">مراجعة الموارد المذكورة أدناه لحل المشكلة التي تواجهها الآن.</span><span class="sxs-lookup"><span data-stu-id="f5839-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="f5839-104">بعض المشاكل الشائعة ودقة الخطوات:</span><span class="sxs-lookup"><span data-stu-id="f5839-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="f5839-105">**الجهاز غير مشفرة خطأ في "مدخل الشركة على الإنترنت":** تتطلب الإصدارات الأحدث من الروبوت، بدءاً v7.0، لا سيما رمز مرور بدء تشغيل للتأكد من أن الجهاز مشفرة بالكامل.</span><span class="sxs-lookup"><span data-stu-id="f5839-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="f5839-106">يتم إيجاد حلول مشتركة لتمكين pin بدء تشغيل أو تشفير الجهاز تماما.</span><span class="sxs-lookup"><span data-stu-id="f5839-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="f5839-107">مراجعة [هذا المستند](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="f5839-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="f5839-108">**فشل أجهزة للتحقق بخدمة إينتوني أو عرض ك "الصحية" في وحدة تحكم المسؤول إينتوني:** قد لا تحقق بعض 4.4 سامسونج وأجهزة 5.5 إلى الخدمة.</span><span class="sxs-lookup"><span data-stu-id="f5839-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="f5839-109">هناك 3 الحلول الممكنة لهذه المشكلة:</span><span class="sxs-lookup"><span data-stu-id="f5839-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="f5839-110">فتح التطبيق "مدخل الشركة إينتوني"، الذي سيبدأ تلقائياً مزامنة جهاز يدوياً.</span><span class="sxs-lookup"><span data-stu-id="f5839-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="f5839-111">تحديث الجهاز إلى 6.0 الروبوت أو أعلى.</span><span class="sxs-lookup"><span data-stu-id="f5839-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="f5839-112">تعطيل "إدارة الذكية سامسونج" من إدارة "مدخل الشركة إينتوني".</span><span class="sxs-lookup"><span data-stu-id="f5839-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="f5839-113">مراجعة [هذا المستند](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) لمزيد من التفاصيل عن هذه المشاكل والحلول.</span><span class="sxs-lookup"><span data-stu-id="f5839-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="f5839-114">**نوع المستخدم ترخيص غير صالح** أو **"المستخدم يتم التعرف على اسم" الخطأ:** يحتاج المستخدم لتعيين ترخيص إينتوني أو نظم الإدارة البيئية.</span><span class="sxs-lookup"><span data-stu-id="f5839-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="f5839-115">مراجعة هذه المستندات لتعيين ترخيص إلى: مدخل مركز مسؤول Office أو Azure.</span><span class="sxs-lookup"><span data-stu-id="f5839-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="f5839-116">موارد إضافية للمساعدة في حل المشكلة:</span><span class="sxs-lookup"><span data-stu-id="f5839-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="f5839-117">استخدام [إينتوني مدخل استكشاف الأخطاء وإصلاحها](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص وحل فشل التسجيل الشائعة.</span><span class="sxs-lookup"><span data-stu-id="f5839-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="f5839-118">مراجعة [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول على مزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="f5839-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="f5839-119">مراجعة [هذا المستند](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) للحصول على قائمة أخطاء الشائعة التي تمنع التسجيل والحلول لكل.</span><span class="sxs-lookup"><span data-stu-id="f5839-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="f5839-120">[التعرف على كيفية تسجيل أجهزة الروبوت في Microsoft إينتوني](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="f5839-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
