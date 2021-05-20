---
title: مشاكل تتعلق بإزالة جهاز تم إيقاف تشغيله أو إيقاف تشغيله من "مخزون الأجهزة"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564000"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="950b9-102">مشاكل تتعلق بإزالة جهاز تم إيقاف تشغيله أو إيقاف تشغيله من "مخزون الأجهزة"</span><span class="sxs-lookup"><span data-stu-id="950b9-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="950b9-103">لا يسمح Microsoft Defender ل Endpoint حاليا بإزالة سجل الجهاز يدويا لجهاز تم إيقاف تشغيله أو إيقاف تشغيله من "مخزون الجهاز".</span><span class="sxs-lookup"><span data-stu-id="950b9-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="950b9-104">لأغراض الأمان، يظل الجهاز في المدخل كسجل تاريخي لمدة تصل إلى 180 يوما.</span><span class="sxs-lookup"><span data-stu-id="950b9-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="950b9-105">ومع ذلك، يتم إزالة بيانات الجهاز وفقا لفترة الاستبقاء التي تم تكوينها.</span><span class="sxs-lookup"><span data-stu-id="950b9-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="950b9-106">**ملاحظة:** يتم تبديل الجهاز غير المستخدم أو المفجوع  تلقائيا إلى حالة "غير نشط" بعد سبعة أيام.</span><span class="sxs-lookup"><span data-stu-id="950b9-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="950b9-107">بالإضافة إلى ذلك، لا يتم حساب الأجهزة غير النشطة في آخر 30 يوما في البيانات التي تعكس درجة التعرض للضوء إدارة المخاطر والثغرات الأمنية أو Microsoft Secure Score للأجهزة.</span><span class="sxs-lookup"><span data-stu-id="950b9-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="950b9-108">إذا كنت لا تزال لا تريد رؤية أجهزة معينة في طريقة عرض "مخزون الجهاز"، فحاول وضع علامة جهاز لتصفية الجهاز الذي تم قطع تشغيله من طريقة عرض "مخزون الجهاز".</span><span class="sxs-lookup"><span data-stu-id="950b9-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="950b9-109">لمزيد من المعلومات، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="950b9-109">For more information, see:</span></span>

[<span data-ttu-id="950b9-110">أجهزة إيقاف التشغيل من خدمة Microsoft Defender لنقطة النهاية</span><span class="sxs-lookup"><span data-stu-id="950b9-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="950b9-111">درجة التعرض للضوء في إدارة المخاطر والثغرات الأمنية</span><span class="sxs-lookup"><span data-stu-id="950b9-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="950b9-112">إصلاح أدوات الاستشعار غير الصحية في Microsoft Defender لنقطة النهاية</span><span class="sxs-lookup"><span data-stu-id="950b9-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="950b9-113">كيفية استخدام العلامات بفعالية (الجزء 1)</span><span class="sxs-lookup"><span data-stu-id="950b9-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="950b9-114">كيفية استخدام العلامات بفعالية (الجزء 2)</span><span class="sxs-lookup"><span data-stu-id="950b9-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="950b9-115">كيفية استخدام العلامات بفعالية (الجزء 3)</span><span class="sxs-lookup"><span data-stu-id="950b9-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




