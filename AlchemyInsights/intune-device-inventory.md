---
title: مخزون الجهاز Intune
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
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438792"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="c2558-102">مخزون الجهاز Intune</span><span class="sxs-lookup"><span data-stu-id="c2558-102">Intune Device Inventory</span></span>

<span data-ttu-id="c2558-103">يوفر شفرة الأجهزة فكرة المسؤول عن الأجهزة الخاضعة للإدارة في Intune على أساس كل جهاز.</span><span class="sxs-lookup"><span data-stu-id="c2558-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="c2558-104">تتضمن المعلومات المعروضة: الأجهزة والتطبيقات المكتشفة وحالة توافق الجهاز وحالة تكوين الجهاز.</span><span class="sxs-lookup"><span data-stu-id="c2558-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="c2558-105">يتم جمع بيانات المخزون للأجهزة والتطبيقات المكتشفة في دورة مدتها سبعة أيام.</span><span class="sxs-lookup"><span data-stu-id="c2558-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="c2558-106">تختلف التطبيقات وعناصر الأجهزة المحددة التي تم الإبلاغ عنها اعتمادًا على نظام تشغيل الجهاز وما إذا كان الجهاز مملوكًا شخصيًا أو مملوكًا للشركات.</span><span class="sxs-lookup"><span data-stu-id="c2558-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="c2558-107">لمزيد من المعلومات، راجع [تفاصيل الجهاز في Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="c2558-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="c2558-108">**الأسئلة المتداولة**</span><span class="sxs-lookup"><span data-stu-id="c2558-108">**FAQ**</span></span>

<span data-ttu-id="c2558-109">س: لا أتلقى قائمة جرد كاملة من التطبيقات الموجودة على أجهزة Windows المسجلين Intune.</span><span class="sxs-lookup"><span data-stu-id="c2558-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="c2558-110">لم لا؟</span><span class="sxs-lookup"><span data-stu-id="c2558-110">Why not?</span></span>

<span data-ttu-id="c2558-111">A: في هذا الوقت، يتم سرد التطبيقات الحديثة فقط لأجهزة الكمبيوتر الشخصية Windows 10 التي تم تعريفها كأجهزة الشركات.</span><span class="sxs-lookup"><span data-stu-id="c2558-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="c2558-112">لا تقوم Intune بتجميع معلومات حول تطبيقات Win32 المثبتة على هذه الأجهزة.</span><span class="sxs-lookup"><span data-stu-id="c2558-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="c2558-113">س: لماذا لا يتم جمع أرقام الهواتف من جميع الأجهزة؟</span><span class="sxs-lookup"><span data-stu-id="c2558-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="c2558-114">A: لا يتم تحديد الهواتف المصنفة على أنها أجهزة الشركة في Intune مع رقم الهاتف الكامل عند تشغيل تقرير مخزون جهاز محمول على سبيل المثال.</span><span class="sxs-lookup"><span data-stu-id="c2558-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="c2558-115">أرقام الهاتف إحضار الجهاز الخاص دائماً جزئياً ملثمين مع العلامات النجمية (\*\*\*\*\* ) ، وتظهر فقط الأرقام الأربعة الأخيرة.</span><span class="sxs-lookup"><span data-stu-id="c2558-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>