---
title: إزالة البيانات ومسح الأجهزة من Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438791"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="42060-102">إزالة البيانات ومسح الأجهزة من Intune</span><span class="sxs-lookup"><span data-stu-id="42060-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="42060-103">يمكن استخدام إجراءات الجهاز "تقاعد" و"مسح الجهاز" عن بعد لإزالة بيانات الشركة التي تديرها Intune أو لإجراء إعادة تعيين المصنع وإعادة الجهاز إلى إعداداته الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="42060-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="42060-104">تسجيل الدخول إلى Microsoft 365 إدارة الأجهزة، ثم انتقل إلى **الأجهزة**  >  **كافة الأجهزة**.</span><span class="sxs-lookup"><span data-stu-id="42060-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="42060-105">حدد الجهاز الذي تريد مسحه.</span><span class="sxs-lookup"><span data-stu-id="42060-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="42060-106">حدد نوع المسح عن بعد الذي تريد القيام به.</span><span class="sxs-lookup"><span data-stu-id="42060-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="42060-107">يحذف التقاعد المعلومات التنظيمية فقط، بينما يقوم المسح الكامل باستعادة الجهاز إلى إعدادات المصنع.</span><span class="sxs-lookup"><span data-stu-id="42060-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="42060-108">حدد **نعم** للتأكيد.</span><span class="sxs-lookup"><span data-stu-id="42060-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="42060-109">حتى انتهاء المسح، تظهر حالة إجراء الجهاز كـ "معلّل معلق".</span><span class="sxs-lookup"><span data-stu-id="42060-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="42060-110">بعد اكتمال الإجراء، لن ترى الجهاز المحمول في قائمة الجهاز المُدار.</span><span class="sxs-lookup"><span data-stu-id="42060-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="42060-111">**ملاحظة** لا يمكن إزالة بيانات الشركة من الأجهزة التي تم الانضمام إليها إلى Azure AD.</span><span class="sxs-lookup"><span data-stu-id="42060-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="42060-112">للحصول على التفاصيل الكاملة لتأثير إجراءات التقاعد والمسح، بما في ذلك ما يتم الاحتفاظ به وما يتم حذفه، راجع [إزالة الأجهزة باستخدام المسح أو التقاعد أو إلغاء تشغيل الجهاز يدويًا](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="42060-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="42060-113">لمسح كافة البيانات من جهاز macOS، راجع [محو كافة البيانات من جهاز macOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="42060-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>