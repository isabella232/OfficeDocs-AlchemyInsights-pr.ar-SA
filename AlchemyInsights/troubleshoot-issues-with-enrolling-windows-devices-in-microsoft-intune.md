---
title: استكشاف المشاكل المتعلقة بتسجيل أجهزة Windows في Microsoft Intune وإصلاحها
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808958"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="437b5-102">استكشاف المشاكل المتعلقة بتسجيل أجهزة Windows في Microsoft Intune وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="437b5-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="437b5-103">راجع الموارد المدرجة أدناه لحل المشكلة الآن.</span><span class="sxs-lookup"><span data-stu-id="437b5-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="437b5-104">بعض رسائل الخطأ الشائعة والخطوات اللازمة لحلها:</span><span class="sxs-lookup"><span data-stu-id="437b5-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="437b5-105">**لا يمكن تثبيت البرنامج، 0x80cf4017:** انتهت صلاحية شهادة حسابك.</span><span class="sxs-lookup"><span data-stu-id="437b5-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="437b5-106">إعادة تنزيل حزمة برامج عميل الكمبيوتر الشخصي في وحدة تحكم مسؤول Intune.</span><span class="sxs-lookup"><span data-stu-id="437b5-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="437b5-107">راجع هذه الوثائق للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="437b5-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="437b5-108">**رمز الخطأ 0x801c0003:** يمكن أن يحدث الخطأ في السيناريوهات التالية:</span><span class="sxs-lookup"><span data-stu-id="437b5-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="437b5-109">لدى المستخدم عدد أجهزة مسجل أكثر من حد الجهاز.</span><span class="sxs-lookup"><span data-stu-id="437b5-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="437b5-110">راجع هذه المستندات [لإزالة جهاز أو](https://docs.microsoft.com/intune/devices-wipe) تغيير حد [الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="437b5-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="437b5-111">يتم تعيين "قد يقوم المستخدمون بضم الأجهزة إلى Azure AD" إلى "بلا".</span><span class="sxs-lookup"><span data-stu-id="437b5-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="437b5-112">قم بتعيينه إلى جميع المستخدمين أو حدده.</span><span class="sxs-lookup"><span data-stu-id="437b5-112">Set it to all or select users.</span></span> <span data-ttu-id="437b5-113">راجع [هذه الوثائق](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="437b5-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="437b5-114">تم تسجيل الجهاز بالفعل من قبل مستخدم آخر.</span><span class="sxs-lookup"><span data-stu-id="437b5-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="437b5-115">إذا كان الأمر كذلك، فإزالة الجهاز من وحدة تحكم Azure Intune أو إلغاء تشغيل الجهاز يدويا قبل المحاولة مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="437b5-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="437b5-116">الجهاز هو Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="437b5-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="437b5-117">يمكن فقط ل Windows 10 Pro و Education و Enterprise SKUs الانضمام إلى Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="437b5-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="437b5-118">موارد إضافية للمساعدة في حل المشكلة:</span><span class="sxs-lookup"><span data-stu-id="437b5-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="437b5-119">استخدم مدخل استكشاف الأخطاء وإصلاحها في [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص حالات فشل التسجيل الشائعة وحلها.</span><span class="sxs-lookup"><span data-stu-id="437b5-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="437b5-120">راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول على مزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="437b5-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="437b5-121">راجع هذه المستندات للحصول على قائمة الأخطاء الشائعة التي تمنع التسجيل والقرارات لكل [منها:](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) دليل استكشاف الأخطاء وإصلاحها ومستند [استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="437b5-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="437b5-122">[تعرف على كيفية تسجيل أجهزة Windows في Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="437b5-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
