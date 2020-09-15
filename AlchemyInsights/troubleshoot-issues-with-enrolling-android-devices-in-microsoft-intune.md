---
title: استكشاف الأخطاء وإصلاحها باستخدام أجهزه Android في Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689941"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="6839b-102">استكشاف الأخطاء وإصلاحها باستخدام أجهزه Android في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6839b-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="6839b-103">راجع الموارد المدرجة أدناه لحل المشكلة الآن.</span><span class="sxs-lookup"><span data-stu-id="6839b-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="6839b-104">بعض المشاكل الشائعة وخطوات الحل:</span><span class="sxs-lookup"><span data-stu-id="6839b-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="6839b-105">**خطا غير مشفر في الجهاز في مدخل الشركة:** تتطلب الإصدارات الأحدث من نظام التشغيل Android ، والتي تبدا ب v 7.0 ، رمز مرور بدء التشغيل للتاكد من ان جهازك مشفر بالبالكامل.</span><span class="sxs-lookup"><span data-stu-id="6839b-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="6839b-106">الحلول الشائعة هي تمكين رمز pin لبدء التشغيل أو تشفير الجهاز بالبالكامل.</span><span class="sxs-lookup"><span data-stu-id="6839b-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="6839b-107">راجع [هذا المستند](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="6839b-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="6839b-108">**فشلت الاجهزه في إيداع الخدمة أو عرضها ك "غير سليم" في وحده تحكم مسؤول Intune:** قد لا تتحقق بعض أجهزه Samsung 4.4 و 5.5 من الخدمة.</span><span class="sxs-lookup"><span data-stu-id="6839b-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="6839b-109">هناك 3 حلول محتمله لهذه المشكلة:</span><span class="sxs-lookup"><span data-stu-id="6839b-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="6839b-110">افتح تطبيق Intune company Portal يدويا ، مما يؤدي إلى بدء مزامنة جهاز تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="6839b-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="6839b-111">تحديث الجهاز إلى Android 6.0 أو إصدار أحدث.</span><span class="sxs-lookup"><span data-stu-id="6839b-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="6839b-112">تعطيل Samsung الاداره الذكية من أداره مدخل شركه Intune.</span><span class="sxs-lookup"><span data-stu-id="6839b-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="6839b-113">راجع [هذا المستند](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) للحصول علي مزيد من التفاصيل حول هذه المشاكل والحلول.</span><span class="sxs-lookup"><span data-stu-id="6839b-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="6839b-114">**نوع ترخيص المستخدم غير صالح** أو **غير معروف اسم المستخدم:** يجب ان يتم تعيين ترخيص Intune أو EMS إلى المستخدم.</span><span class="sxs-lookup"><span data-stu-id="6839b-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="6839b-115">راجع هذه المستندات لتعيين ترخيص عبر: مركز أداره Office أو مدخل Azure.</span><span class="sxs-lookup"><span data-stu-id="6839b-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="6839b-116">موارد اضافيه للمساعدة في حل المشكلة:</span><span class="sxs-lookup"><span data-stu-id="6839b-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="6839b-117">استخدام [مدخل Intune استكشاف الأخطاء وإصلاحها](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص فشل التسجيل الشائع وتصحيحه.</span><span class="sxs-lookup"><span data-stu-id="6839b-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="6839b-118">راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول علي مزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="6839b-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="6839b-119">راجع [هذا المستند](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) للحصول علي قائمه بالأخطاء الشائعة التي تمنع التسجيل والحلول لكل منها.</span><span class="sxs-lookup"><span data-stu-id="6839b-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="6839b-120">[تعرف علي كيفيه تسجيل أجهزه Android في Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="6839b-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
