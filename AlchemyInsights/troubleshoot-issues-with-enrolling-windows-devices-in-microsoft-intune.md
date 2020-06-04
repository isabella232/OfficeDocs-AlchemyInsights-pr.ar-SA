---
title: استكشاف المشاكل المتعلقة بتسجيل أجهزة Windows في Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665819"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="024c9-102">استكشاف المشاكل المتعلقة بتسجيل أجهزة Windows في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="024c9-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="024c9-103">راجع الموارد المذكورة أدناه لحل مشكلتك الآن.</span><span class="sxs-lookup"><span data-stu-id="024c9-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="024c9-104">بعض رسائل الخطأ الشائعة وخطوات الدقة:</span><span class="sxs-lookup"><span data-stu-id="024c9-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="024c9-105">**لا يمكن تثبيت البرنامج، 0x80cf4017:** انتهت صلاحية شهادة حسابك.</span><span class="sxs-lookup"><span data-stu-id="024c9-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="024c9-106">إعادة تحميل حزمة برامج عميل الكمبيوتر في وحدة تحكم الإدارة Intune.</span><span class="sxs-lookup"><span data-stu-id="024c9-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="024c9-107">راجع هذه الوثائق لمزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="024c9-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="024c9-108">**رمز الخطأ 0x801c0003:** يمكن أن يحدث الخطأ في السيناريوهات التالية:</span><span class="sxs-lookup"><span data-stu-id="024c9-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="024c9-109">لدى المستخدم أجهزة أكثر تسجيلًا من حد الجهاز.</span><span class="sxs-lookup"><span data-stu-id="024c9-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="024c9-110">راجع هذه المستندات [لإزالة جهاز](https://docs.microsoft.com/intune/devices-wipe) أو تغيير [حد الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="024c9-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="024c9-111">"قد ينضم المستخدمون إلى الأجهزة إلى Azure AD" تم تعيينه إلى "لا شيء".</span><span class="sxs-lookup"><span data-stu-id="024c9-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="024c9-112">قم بتعيينها إلى كافة المستخدمين أو حددها.</span><span class="sxs-lookup"><span data-stu-id="024c9-112">Set it to all or select users.</span></span> <span data-ttu-id="024c9-113">راجع [هذه الوثائق](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) لمزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="024c9-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="024c9-114">تم تسجيل الجهاز بالفعل من قبل مستخدم آخر.</span><span class="sxs-lookup"><span data-stu-id="024c9-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="024c9-115">إذا كان الأمر كذلك، قم بإزالة الجهاز من وحدة تحكم Azure Intune أو قم بإلغاء تسجيل الجهاز يدويًا قبل المحاولة مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="024c9-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="024c9-116">الجهاز هو ويندوز 10 الرئيسية.</span><span class="sxs-lookup"><span data-stu-id="024c9-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="024c9-117">يمكن فقط لـ Windows 10 Pro والتعليم والشركات الصغيرة والمتوسطة الانضمام إلى Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="024c9-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="024c9-118">موارد إضافية للمساعدة في حل مشكلتك:</span><span class="sxs-lookup"><span data-stu-id="024c9-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="024c9-119">استخدم [بوابة استكشاف الأخطاء وإصلاحها Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص حالات فشل التسجيل الشائعة وحلها.</span><span class="sxs-lookup"><span data-stu-id="024c9-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="024c9-120">راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) لمزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="024c9-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="024c9-121">راجع هذه المستندات للحصول على قائمة من الأخطاء الشائعة التي تمنع التسجيل والحلول لكل: [دليل استكشاف الأخطاء وإصلاحها](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) [ومستند استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="024c9-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="024c9-122">[تعرّف على كيفية تسجيل أجهزة Windows في Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="024c9-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
