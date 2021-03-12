---
title: استكشاف المشاكل المتعلقة بتسجيل أجهزة Android في Microsoft Intune وإصلاحها
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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708985"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="723d3-102">استكشاف المشاكل المتعلقة بتسجيل أجهزة Android في Microsoft Intune وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="723d3-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="723d3-103">راجع الموارد المدرجة أدناه لحل المشكلة الآن.</span><span class="sxs-lookup"><span data-stu-id="723d3-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="723d3-104">بعض المشاكل الشائعة والخطوات اللازمة لحلها:</span><span class="sxs-lookup"><span data-stu-id="723d3-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="723d3-105">**خطأ "الجهاز غير مشفر" في "مدخل الشركة":** تتطلب الإصدارات الأحدث من Android، لا سيما التي تبدأ ب v7.0، رمز مرور بدء التشغيل للتأكد من تشفير جهازك بشكل كامل.</span><span class="sxs-lookup"><span data-stu-id="723d3-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="723d3-106">الحلول الشائعة هي تمكين تثبيت بدء التشغيل أو تشفير الجهاز بالكامل.</span><span class="sxs-lookup"><span data-stu-id="723d3-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="723d3-107">راجع [هذا المستند](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="723d3-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="723d3-108">تفشل الأجهزة في تسجيل الدخول باستخدام خدمة Intune أو عرضها على أنها **"غير صحية" في وحدة تحكم مسؤول Intune:** قد لا تدقق بعض أجهزة Samsung 4.4 و5.5 في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="723d3-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="723d3-109">هناك 3 حلول محتملة لهذه المشكلة:</span><span class="sxs-lookup"><span data-stu-id="723d3-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="723d3-110">افتح تطبيق Intune Company Portal يدويا، مما يؤدي إلى بدء مزامنة الجهاز تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="723d3-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="723d3-111">تحديث الجهاز إلى Android 6.0 أو إصدار أحدث.</span><span class="sxs-lookup"><span data-stu-id="723d3-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="723d3-112">قم بتعطيل Samsung Smart Manager من إدارة مدخل شركة Intune.</span><span class="sxs-lookup"><span data-stu-id="723d3-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="723d3-113">راجع [هذا المستند](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) للحصول على مزيد من التفاصيل حول هذه المشاكل والقرارات.</span><span class="sxs-lookup"><span data-stu-id="723d3-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="723d3-114">**خطأ "نوع ترخيص** المستخدم غير صالح" أو "اسم المستخدم غير متعرف **عليه":** يجب تعيين ترخيص Intune أو EMS للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="723d3-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="723d3-115">راجع هذه المستندات لتعيين ترخيص من خلال: مركز إدارة Office أو مدخل Azure.</span><span class="sxs-lookup"><span data-stu-id="723d3-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="723d3-116">موارد إضافية للمساعدة في حل المشكلة:</span><span class="sxs-lookup"><span data-stu-id="723d3-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="723d3-117">استخدم مدخل استكشاف الأخطاء وإصلاحها في [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص حالات الفشل الشائعة في التسجيل وحلها.</span><span class="sxs-lookup"><span data-stu-id="723d3-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="723d3-118">راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول على مزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="723d3-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="723d3-119">راجع [هذا المستند](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) للحصول على قائمة الأخطاء الشائعة التي تمنع تسجيل كل منها والقرارات المتعلقة به.</span><span class="sxs-lookup"><span data-stu-id="723d3-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="723d3-120">[تعرف على كيفية تسجيل أجهزة Android في Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="723d3-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
