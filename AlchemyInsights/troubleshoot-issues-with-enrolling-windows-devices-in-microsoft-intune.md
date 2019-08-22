---
title: استكشاف مشكلات تسجيل أجهزة Windows في Microsoft إينتوني
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559612"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="2f89f-102">استكشاف مشكلات تسجيل أجهزة Windows في Microsoft إينتوني</span><span class="sxs-lookup"><span data-stu-id="2f89f-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="2f89f-103">مراجعة الموارد المذكورة أدناه لحل المشكلة التي تواجهها الآن.</span><span class="sxs-lookup"><span data-stu-id="2f89f-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="2f89f-104">بعض رسائل الخطأ الشائعة ودقة الخطوات:</span><span class="sxs-lookup"><span data-stu-id="2f89f-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="2f89f-105">**لا يمكن تثبيت البرنامج، 0x80cf4017:** انتهت صلاحية شهادة الحساب الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="2f89f-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="2f89f-106">إعادة تحميل حزمة برامج الكمبيوتر العميل في وحدة تحكم الإدارة إينتوني.</span><span class="sxs-lookup"><span data-stu-id="2f89f-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="2f89f-107">مراجعة هذه الوثائق للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="2f89f-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="2f89f-108">**رمز الخطأ 0x801c0003:** يمكن أن يحدث الخطأ في السيناريوهات التالية:</span><span class="sxs-lookup"><span data-stu-id="2f89f-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="2f89f-109">ليس لدى المستخدم المزيد من أجهزة تسجيل من حد الجهاز.</span><span class="sxs-lookup"><span data-stu-id="2f89f-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="2f89f-110">مراجعة هذه المستندات [إزالة جهاز](https://docs.microsoft.com/intune/devices-wipe) أو [تغيير حد الجهاز](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="2f89f-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="2f89f-111">يتم تعيين "المستخدمين قد وصل الأجهزة لإعلان Azure" إلى "بلا".</span><span class="sxs-lookup"><span data-stu-id="2f89f-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="2f89f-112">تعيين للكل أو تحديد المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="2f89f-112">Set it to all or select users.</span></span> <span data-ttu-id="2f89f-113">مراجعة [هذه الوثائق](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="2f89f-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="2f89f-114">تم تسجيل الجهاز مسبقاً من قبل مستخدم آخر.</span><span class="sxs-lookup"><span data-stu-id="2f89f-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="2f89f-115">إذا كان الأمر كذلك، إزالة الجهاز من وحدة Azure إينتوني أو أونينرول الجهاز يدوياً قبل المحاولة مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="2f89f-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="2f89f-116">الجهاز هو 10 Windows Home.</span><span class="sxs-lookup"><span data-stu-id="2f89f-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="2f89f-117">وصل فقط Windows 10 Pro والتعليم ووحدات Sku المؤسسة Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2f89f-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="2f89f-118">موارد إضافية للمساعدة في حل المشكلة:</span><span class="sxs-lookup"><span data-stu-id="2f89f-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="2f89f-119">استخدام [إينتوني مدخل استكشاف الأخطاء وإصلاحها](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) لتشخيص وحل فشل التسجيل الشائعة.</span><span class="sxs-lookup"><span data-stu-id="2f89f-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="2f89f-120">مراجعة [هذا المستند](https://docs.microsoft.com/intune/help-desk-operators) للحصول على مزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="2f89f-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="2f89f-121">مراجعة هذه الوثائق للحصول على قائمة أخطاء الشائعة التي تمنع التسجيل والحلول لكل: [دليل استكشاف الأخطاء وإصلاحها](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) و [مستند استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="2f89f-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="2f89f-122">[التعرف على كيفية تسجيل أجهزة Windows في Microsoft إينتوني](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="2f89f-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
