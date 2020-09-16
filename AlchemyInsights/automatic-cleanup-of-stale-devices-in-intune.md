---
title: التنظيف التلقائي للاجهزه التالفة في Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715008"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="bba85-102">التنظيف التلقائي للاجهزه التالفة في Intune</span><span class="sxs-lookup"><span data-stu-id="bba85-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="bba85-103">يسمح Intune للمسؤول بتكوين فتره زمنيه بين 90 و 270 يوما ، وذلك بعد الذي تتم أزاله الاجهزه التالفة من الخدمة.</span><span class="sxs-lookup"><span data-stu-id="bba85-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="bba85-104">هذا الاعداد واسع النطاق وبمجرد تنشيطه ، فانه سيظهر حيز التنفيذ مباشره.</span><span class="sxs-lookup"><span data-stu-id="bba85-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="bba85-105">يتم حذف اي أجهزه لم يتم إيداعها في خادم Intune لمده تتجاوز الاعداد بشكل دائم.</span><span class="sxs-lookup"><span data-stu-id="bba85-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="bba85-106">**ملاحظه** فقط كائنات جهاز MDM هي المؤهلة لاجراء التنظيف هذا.</span><span class="sxs-lookup"><span data-stu-id="bba85-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="bba85-107">يتم استبعاد كائنات جهاز EAS فقط.</span><span class="sxs-lookup"><span data-stu-id="bba85-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="bba85-108">للحصول علي مزيد من المعلومات حول الوقت الذي يصبح فيه الجهاز مؤهلا للحذف استنادا إلى اعداد الجهاز وحالته التي:</span><span class="sxs-lookup"><span data-stu-id="bba85-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="bba85-109">الاعداد: **حذف الاجهزه بعد تاريخ الإيداع الأخير: نعم (بعض القيمة (N) في الأيام المحددة)**</span><span class="sxs-lookup"><span data-stu-id="bba85-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="bba85-110">بالاستناد إلى القيمة (N) التي تم تكوينها في الاعداد ، تقوم خدمه Intune بحذف الجهاز في الأيام المحددة بعد إيداعه آخر مره بنجاح.</span><span class="sxs-lookup"><span data-stu-id="bba85-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="bba85-111">اعداد:  **حذف الاجهزه بعد تاريخ الإيداع الأخير: لا**</span><span class="sxs-lookup"><span data-stu-id="bba85-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="bba85-112">180 يوما بعد انتهاء صلاحيه شهادة الجهاز ولم يتم تجديدها ، يتم حذف الجهاز.</span><span class="sxs-lookup"><span data-stu-id="bba85-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="bba85-113">**ملاحظه** في كلتا الحالتين ، يجب تسجيل الجهاز بنجاح في Intune.</span><span class="sxs-lookup"><span data-stu-id="bba85-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="bba85-114">يحدث التسجيل خلال الجهاز الأول الذي يتم إيداعه باستخدام خدمه Intune.</span><span class="sxs-lookup"><span data-stu-id="bba85-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="bba85-115">إذا كان الجهاز تسجيل بنجاح إلى Intune ولكنه لا يتم تسجيله في Intune ، سيتم حذف الجهاز بعد 270 يوما بعد التسجيل.</span><span class="sxs-lookup"><span data-stu-id="bba85-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="bba85-116">(90 يوما لوضع علامة علي الجهاز كملغي ، ثم 180 يوما آخر لحذف السجل.)</span><span class="sxs-lookup"><span data-stu-id="bba85-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="bba85-117">لا توجد اي اليه حاليا في وحده تحكم Intune لإنشاء تاريخ انتهاء صلاحيه شهادة الجهاز لأي جهاز محدد.</span><span class="sxs-lookup"><span data-stu-id="bba85-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>