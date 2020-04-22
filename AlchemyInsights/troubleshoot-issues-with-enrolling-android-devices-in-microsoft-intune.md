---
title: استكشاف المشاكل المتعلقة بتسجيل أجهزة Android في Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759607"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="bc72b-102">استكشاف المشاكل المتعلقة بتسجيل أجهزة Android في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bc72b-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="bc72b-103">راجع الموارد المذكورة أدناه لحل مشكلتك الآن.</span><span class="sxs-lookup"><span data-stu-id="bc72b-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="bc72b-104">بعض القضايا الشائعة وخطوات الحل:</span><span class="sxs-lookup"><span data-stu-id="bc72b-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="bc72b-105">**خطأ غير مشفر في الجهاز في بوابة الشركة:** تتطلب الإصدارات الأحدث من Android ، خاصة ً بدءًا من v7.0 ، رمز مرور بدء التشغيل للتأكد من تشفير جهازك بالكامل.</span><span class="sxs-lookup"><span data-stu-id="bc72b-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="bc72b-106">الحلول الشائعة هي تمكين دبوس بدء التشغيل أو تشفير الجهاز بالكامل.</span><span class="sxs-lookup"><span data-stu-id="bc72b-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="bc72b-107">راجع [هذا المستند](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) لمزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="bc72b-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="bc72b-108">**تفشل الأجهزة في تسجيل الوصول باستخدام خدمة Intune أو عرضها كـ "غير صحية" في وحدة تحكم إدارة Intune:** قد لا تحقق بعض أجهزة سامسونج 4.4 و5.5 في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="bc72b-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="bc72b-109">هناك 3 حلول ممكنة لهذه المشكلة:</span><span class="sxs-lookup"><span data-stu-id="bc72b-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="bc72b-110">افتح تطبيق بوابة شركة Intune يدويًا، والذي سيبدأ مزامنة الجهاز تلقائيًا.</span><span class="sxs-lookup"><span data-stu-id="bc72b-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="bc72b-111">تحديث الجهاز إلى الروبوت 6.0 أو أعلى.</span><span class="sxs-lookup"><span data-stu-id="bc72b-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="bc72b-112">تعطيل مدير سامسونج الذكي من إدارة بوابة شركة Intune.</span><span class="sxs-lookup"><span data-stu-id="bc72b-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="bc72b-113">راجع [هذه الوثيقة](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) لمزيد من التفاصيل حول هذه القضايا والقرارات.</span><span class="sxs-lookup"><span data-stu-id="bc72b-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="bc72b-114">**خطأ غير صالح** أو اسم المستخدم غير معروف نوع ترخيص **المستخدم:** يحتاج المستخدم إلى تعيين ترخيص Intune أو EMS.</span><span class="sxs-lookup"><span data-stu-id="bc72b-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="bc72b-115">راجع هذه المستندات لتعيين ترخيص من خلال: مركز Office Admin أو بوابة Azure.</span><span class="sxs-lookup"><span data-stu-id="bc72b-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="bc72b-116">موارد إضافية للمساعدة في حل مشكلتك:</span><span class="sxs-lookup"><span data-stu-id="bc72b-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="bc72b-117">استخدم [بوابة استكشاف الأخطاء وإصلاحها Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص حالات فشل التسجيل الشائعة وحلها.</span><span class="sxs-lookup"><span data-stu-id="bc72b-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="bc72b-118">راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) لمزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="bc72b-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="bc72b-119">راجع [هذا المستند](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) للحصول على قائمة بالأخطاء الشائعة التي تمنع التسجيل والحلول لكل منها.</span><span class="sxs-lookup"><span data-stu-id="bc72b-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="bc72b-120">[تعرّف على كيفية تسجيل أجهزة Android في Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="bc72b-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
