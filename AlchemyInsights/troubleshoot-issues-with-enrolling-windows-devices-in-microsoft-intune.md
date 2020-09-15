---
title: استكشاف الأخطاء وإصلاحها في تسجيل أجهزه Windows في Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658865"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="97cee-102">استكشاف الأخطاء وإصلاحها في تسجيل أجهزه Windows في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="97cee-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="97cee-103">راجع الموارد المدرجة أدناه لحل المشكلة الآن.</span><span class="sxs-lookup"><span data-stu-id="97cee-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="97cee-104">بعض رسائل الخطا الشائعة وخطوات الدقة:</span><span class="sxs-lookup"><span data-stu-id="97cee-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="97cee-105">**لا يمكن تثبيت البرنامج ، 0x80cf4017:** انتهت صلاحيه شهادة حسابك.</span><span class="sxs-lookup"><span data-stu-id="97cee-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="97cee-106">قم باعاده تنزيل حزمه برامج عميل الكمبيوتر الشخصي في وحده تحكم مسؤول Intune.</span><span class="sxs-lookup"><span data-stu-id="97cee-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="97cee-107">راجع هذه الوثائق للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="97cee-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="97cee-108">**رمز الخطا 0x801c0003:** يمكن ان يحدث الخطا في السيناريوهات التالية:</span><span class="sxs-lookup"><span data-stu-id="97cee-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="97cee-109">يملك المستخدم المزيد من الاجهزه التي تم تسجيلها من حد الجهاز.</span><span class="sxs-lookup"><span data-stu-id="97cee-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="97cee-110">راجع هذه المستندات [لأزاله جهاز](https://docs.microsoft.com/intune/devices-wipe) أو [تغيير حد الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="97cee-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="97cee-111">"يمكن ان ينضم المستخدمون إلى الاجهزه التي تم تعيينها إلى" بلا ".</span><span class="sxs-lookup"><span data-stu-id="97cee-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="97cee-112">قم بتعيينه إلى جميع المستخدمين أو حددهم.</span><span class="sxs-lookup"><span data-stu-id="97cee-112">Set it to all or select users.</span></span> <span data-ttu-id="97cee-113">راجع [هذه الوثائق](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="97cee-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="97cee-114">تم تسجيل الجهاز بالفعل من قبل مستخدم آخر.</span><span class="sxs-lookup"><span data-stu-id="97cee-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="97cee-115">إذا كانت هذه هي الحالة ، فقم بازاله الجهاز من وحده التحكم Azure Intune أو أونينرول الجهاز يدويا قبل المحاولة مره أخرى.</span><span class="sxs-lookup"><span data-stu-id="97cee-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="97cee-116">الجهاز هو Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="97cee-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="97cee-117">يمكن لنظام التشغيل Windows 10 Pro والتعليم ووحدات Sku للمؤسسة الانضمام إلى Azure Active directory.</span><span class="sxs-lookup"><span data-stu-id="97cee-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="97cee-118">موارد اضافيه للمساعدة في حل المشكلة:</span><span class="sxs-lookup"><span data-stu-id="97cee-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="97cee-119">استخدام [مدخل Intune استكشاف الأخطاء وإصلاحها](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص فشل التسجيل الشائع وتصحيحه.</span><span class="sxs-lookup"><span data-stu-id="97cee-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="97cee-120">راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول علي مزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="97cee-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="97cee-121">راجع المستندات التالية للحصول علي قائمه بالأخطاء الشائعة التي تمنع التسجيل والحلول لكل منها: [دليل استكشاف الأخطاء](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) وإصلاحها [واستكشاف أخطاء المستند](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="97cee-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="97cee-122">[تعرف علي كيفيه تسجيل أجهزه Windows في Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="97cee-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
