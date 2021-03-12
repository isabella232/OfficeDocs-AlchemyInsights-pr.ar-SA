---
title: استكشاف المشاكل المتعلقة بتسجيل أجهزة Windows في Microsoft Intune وإصلاحها
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
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708877"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="e6d13-102">استكشاف المشاكل المتعلقة بتسجيل أجهزة Windows في Microsoft Intune وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="e6d13-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="e6d13-103">راجع الموارد المدرجة أدناه لحل المشكلة الآن.</span><span class="sxs-lookup"><span data-stu-id="e6d13-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="e6d13-104">بعض رسائل الخطأ الشائعة وبعض خطوات الحل:</span><span class="sxs-lookup"><span data-stu-id="e6d13-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="e6d13-105">**يتعذر تثبيت البرنامج، 0x80cf4017:** انتهت صلاحية شهادة حسابك.</span><span class="sxs-lookup"><span data-stu-id="e6d13-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="e6d13-106">إعادة تنزيل حزمة برامج عميل الكمبيوتر الشخصي في وحدة تحكم مسؤول Intune.</span><span class="sxs-lookup"><span data-stu-id="e6d13-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="e6d13-107">راجع هذه الوثائق للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="e6d13-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="e6d13-108">**رمز الخطأ 0x801c0003:** يمكن أن يحدث الخطأ في السيناريوهات التالية:</span><span class="sxs-lookup"><span data-stu-id="e6d13-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="e6d13-109">لدى المستخدم عدد من الأجهزة مسجل أكثر من حد الجهاز.</span><span class="sxs-lookup"><span data-stu-id="e6d13-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="e6d13-110">راجع هذه المستندات [لإزالة جهاز](https://docs.microsoft.com/intune/devices-wipe) أو [تغيير حد الجهاز.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="e6d13-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="e6d13-111">يتم تعيين "قد يقوم المستخدمون بضم الأجهزة إلى Azure AD" إلى "بلا".</span><span class="sxs-lookup"><span data-stu-id="e6d13-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="e6d13-112">قم بتعيينه إلى جميع المستخدمين أو تحديدهم.</span><span class="sxs-lookup"><span data-stu-id="e6d13-112">Set it to all or select users.</span></span> <span data-ttu-id="e6d13-113">راجع [هذه الوثائق](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="e6d13-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="e6d13-114">تم تسجيل الجهاز بالفعل من قبل مستخدم آخر.</span><span class="sxs-lookup"><span data-stu-id="e6d13-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="e6d13-115">إذا كان الأمر كذلك، فإزالة الجهاز من وحدة تحكم Azure Intune أو إلغاء تشغيل الجهاز يدويا قبل إعادة المحاولة.</span><span class="sxs-lookup"><span data-stu-id="e6d13-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="e6d13-116">الجهاز هو Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="e6d13-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="e6d13-117">يمكن فقط ل Windows 10 Pro و Education و Enterprise SK الانضمام إلى Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e6d13-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="e6d13-118">موارد إضافية للمساعدة في حل المشكلة:</span><span class="sxs-lookup"><span data-stu-id="e6d13-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="e6d13-119">استخدم مدخل استكشاف الأخطاء وإصلاحها في [Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص حالات الفشل الشائعة في التسجيل وحلها.</span><span class="sxs-lookup"><span data-stu-id="e6d13-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e6d13-120">راجع [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول على مزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="e6d13-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="e6d13-121">راجع هذه المستندات للحصول على قائمة الأخطاء الشائعة التي تمنع التسجيل والقرارات لكل [منها:](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) دليل استكشاف الأخطاء وإصلاحها ومستند استكشاف [الأخطاء وإصلاحها.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="e6d13-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="e6d13-122">[تعرف على كيفية تسجيل أجهزة Windows في Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="e6d13-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
