---
title: التنظيف التلقائي للأجهزة التي لا معنى لها في Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554710"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="a3aec-102">التنظيف التلقائي للأجهزة التي لا معنى لها في Intune</span><span class="sxs-lookup"><span data-stu-id="a3aec-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="a3aec-103">Intune يسمح للمسؤول لتكوين الفاصل الزمني بين 90 و 270 يوما ، وبعد ذلك يتم إزالة الأجهزة التي لا معنى لها من الخدمة.</span><span class="sxs-lookup"><span data-stu-id="a3aec-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="a3aec-104">هذا الإعداد هو المنظمة واسعة وبمجرد تفعيلها يدخل حيز التنفيذ على الفور.</span><span class="sxs-lookup"><span data-stu-id="a3aec-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="a3aec-105">يتم حذف أي أجهزة لم يتم إيداعها في خادم Intune لفترة تتجاوز الإعداد بشكل دائم.</span><span class="sxs-lookup"><span data-stu-id="a3aec-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="a3aec-106">**ملاحظة** كائنات جهاز MDM هي فقط المؤهلة لإجراء التنظيف هذا.</span><span class="sxs-lookup"><span data-stu-id="a3aec-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="a3aec-107">يتم استبعاد كائنات الجهاز فقط EAS.</span><span class="sxs-lookup"><span data-stu-id="a3aec-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="a3aec-108">للحصول على معلومات إضافية حول الوقت الذي يصبح فيه الجهاز مؤهلاً للحذف بناءً على إعداد تنظيف الجهاز و"حالته":</span><span class="sxs-lookup"><span data-stu-id="a3aec-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="a3aec-109">الإعداد: **حذف الأجهزة بعد تاريخ آخر تسجيل للانقـان: نعم (بعض القيمة (N) في الأيام المحددة)**</span><span class="sxs-lookup"><span data-stu-id="a3aec-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="a3aec-110">استناداً إلى القيمة (N) التي تم تكوينها في الإعداد، تقوم خدمة Intune بحذف الجهاز في الأيام المحددة بعد أن تحقق بنجاح.</span><span class="sxs-lookup"><span data-stu-id="a3aec-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="a3aec-111">الإعداد: **حذف الأجهزة بعد تاريخ آخر تسجيل الوصول: لا**</span><span class="sxs-lookup"><span data-stu-id="a3aec-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="a3aec-112">بعد 180 يوماً من انتهاء صلاحية شهادة الجهاز وعدم تجديدها، يتم حذف الجهاز.</span><span class="sxs-lookup"><span data-stu-id="a3aec-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="a3aec-113">**ملاحظة** في كلتا الحالتين، يجب أن يتم تسجيل الجهاز بنجاح في Intune.</span><span class="sxs-lookup"><span data-stu-id="a3aec-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="a3aec-114">يحدث التسجيل أثناء تسجيل الجهاز الأول مع خدمة Intune.</span><span class="sxs-lookup"><span data-stu-id="a3aec-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="a3aec-115">إذا كان الجهاز يسجل بنجاح إلى إينتوني ولكن لا تصبح Intune مسجلة، يتم حذف الجهاز 270 يوما بعد التسجيل.</span><span class="sxs-lookup"><span data-stu-id="a3aec-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="a3aec-116">(90 يوماً لوضع علامة على الجهاز كما إبطال، ثم 180 يوماً أخرى لحذف السجل.)</span><span class="sxs-lookup"><span data-stu-id="a3aec-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="a3aec-117">لا توجد آلية حالياً في وحدة التحكم Intune لتحديد تاريخ انتهاء صلاحية شهادة الجهاز لأي جهاز معين.</span><span class="sxs-lookup"><span data-stu-id="a3aec-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>