---
title: مخزون جهاز Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667865"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="9cbea-102">مخزون جهاز Intune</span><span class="sxs-lookup"><span data-stu-id="9cbea-102">Intune Device Inventory</span></span>

<span data-ttu-id="9cbea-103">توفر النصليه الاجهزه المسؤول الذي يمكنك استخدامه لمعرفه الاجهزه ضمن الاداره في Intune علي أساس الجهاز.</span><span class="sxs-lookup"><span data-stu-id="9cbea-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="9cbea-104">تتضمن المعلومات المعروضة: الاجهزه والتطبيقات التي تم اكتشافها وحاله توافق الاجهزه وحاله تكوين الجهاز.</span><span class="sxs-lookup"><span data-stu-id="9cbea-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="9cbea-105">يتم جمع بيانات المخزون للاجهزه والتطبيقات التي تم اكتشافها في دوره سبعه أيام.</span><span class="sxs-lookup"><span data-stu-id="9cbea-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="9cbea-106">تختلف التطبيقات والعناصر المحددة للاجهزه التي تم الإبلاغ عنها وفقا لنظام تشغيل الجهاز وما إذا كان الجهاز شخصيا أو مملوكا للشركة.</span><span class="sxs-lookup"><span data-stu-id="9cbea-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="9cbea-107">لمزيد من المعلومات ، راجع [الاطلاع علي تفاصيل الجهاز في Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="9cbea-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="9cbea-108">**الأسئلة المتداولة**</span><span class="sxs-lookup"><span data-stu-id="9cbea-108">**FAQ**</span></span>

<span data-ttu-id="9cbea-109">س: لا أتلقى قائمه جرد كامله من التطبيقات المتوفرة علي أجهزه Windows التي تم تسجيلها من قبل Intune.</span><span class="sxs-lookup"><span data-stu-id="9cbea-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="9cbea-110">لم لا؟</span><span class="sxs-lookup"><span data-stu-id="9cbea-110">Why not?</span></span>

<span data-ttu-id="9cbea-111">ج: في الوقت الحالي ، يتم فقط سرد التطبيقات الحديثة لأجهزه الكمبيوتر التي تعمل بنظام Windows 10 التي تم تعريفها كاجهزه مشتركه.</span><span class="sxs-lookup"><span data-stu-id="9cbea-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="9cbea-112">لا يجمع Intune المعلومات حول تطبيقات Win32 المثبتة علي هذه الاجهزه.</span><span class="sxs-lookup"><span data-stu-id="9cbea-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="9cbea-113">س: لم يتم جمع أرقام الهواتف من كل الاجهزه ؟</span><span class="sxs-lookup"><span data-stu-id="9cbea-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="9cbea-114">ج: لم يتم تعريف الهواتف التي تم تصنيفها كاجهزه مشتركه في Intune باستخدام رقم الهاتف الكامل الخاص بها ، علي سبيل المثال ، يمكنك تشغيل تقرير مخزون جهاز محمول.</span><span class="sxs-lookup"><span data-stu-id="9cbea-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="9cbea-115">يتم دائما تزويد أرقام هواتف الاجهزه الخاصة بالجهاز بعلامات نجميه (\* \* \* \*) ، وإظهار الأرقام الاربعه الاخيره فقط.</span><span class="sxs-lookup"><span data-stu-id="9cbea-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>