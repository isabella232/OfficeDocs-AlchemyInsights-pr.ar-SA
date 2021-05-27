---
title: حالة مستشعر التحقق من نقطة نهاية Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676026"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="3ca23-102">حالة مستشعر التحقق من نقطة نهاية Defender</span><span class="sxs-lookup"><span data-stu-id="3ca23-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="3ca23-103">توجد **لوحة "الأجهزة التي** بها مشاكل المستشعر" على لوحة معلومات "عمليات الأمان".</span><span class="sxs-lookup"><span data-stu-id="3ca23-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="3ca23-104">توفر هذه اللوحة معلومات حول قدرة الجهاز الفردي على توفير بيانات المستشعر والتواصل مع خدمة Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="3ca23-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="3ca23-105">كما أنها تقوم بلتقارير حول عدد الأجهزة التي تتطلب الانتباه وتساعدك على تحديد الأجهزة التي بها مشاكل واتخاذ الإجراءات اللازمة لتصحيح المشاكل المعروفة.</span><span class="sxs-lookup"><span data-stu-id="3ca23-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="3ca23-106">يوفر مؤشرا الحالة على اللوحة معلومات حول عدد الأجهزة التي لا تبلغ الخدمة بشكل صحيح:</span><span class="sxs-lookup"><span data-stu-id="3ca23-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="3ca23-107">**تم تكوينه بشكل خاطئ** الأجهزة التي قد تقوم جزئيا بالإبلاغ عن بيانات المستشعر لخدمة Defender for Endpoint وقد تكون بها أخطاء تكوين تحتاج إلى تصحيح.</span><span class="sxs-lookup"><span data-stu-id="3ca23-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="3ca23-108">**غير نشط** الأجهزة التي توقفت عن إعداد التقارير إلى خدمة Defender for Endpoint لأكثر من سبعة أيام في الشهر الماضي.</span><span class="sxs-lookup"><span data-stu-id="3ca23-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="3ca23-109">يؤدي النقر فوق أي من المجموعات إلى توجيهك إلى قائمة الأجهزة، التي تمت تصفيتها وفقا اختياراتك.</span><span class="sxs-lookup"><span data-stu-id="3ca23-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="3ca23-110">في قائمة الأجهزة، يمكنك تصفية قائمة حالة الصحة حسب الحالة التالية:</span><span class="sxs-lookup"><span data-stu-id="3ca23-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="3ca23-111">**نشط** الأجهزة التي تقدم تقارير نشطة إلى خدمة Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="3ca23-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="3ca23-112">**تم تكوينه بشكل خاطئ** الأجهزة التي قد تقوم جزئيا بالإبلاغ عن بيانات المستشعر لخدمة Defender for Endpoint ولكن بها أخطاء تكوين يجب تصحيحها.</span><span class="sxs-lookup"><span data-stu-id="3ca23-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="3ca23-113">يمكن أن يكون للأجهزة التي تم تكوينها بشكل خاطئ مشكلة واحدة أو مجموعة من المشاكل التالية:</span><span class="sxs-lookup"><span data-stu-id="3ca23-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="3ca23-114">لا توجد بيانات استشعار - توقفت الأجهزة عن إرسال بيانات المستشعر.</span><span class="sxs-lookup"><span data-stu-id="3ca23-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="3ca23-115">يمكن تشغيل تنبيهات محدودة من الجهاز.</span><span class="sxs-lookup"><span data-stu-id="3ca23-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="3ca23-116">ضعف الاتصالات - ضعف القدرة على التواصل مع الجهاز.</span><span class="sxs-lookup"><span data-stu-id="3ca23-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="3ca23-117">قد لا يعمل إرسال الملفات للتحليل العميق وحظر الملفات وعزل الجهاز عن الشبكة والإجراءات الأخرى التي تتطلب التواصل مع الجهاز.</span><span class="sxs-lookup"><span data-stu-id="3ca23-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="3ca23-118">**غير نشط** الأجهزة التي توقفت عن إعداد التقارير إلى خدمة Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="3ca23-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="3ca23-119">يمكنك تنزيل القائمة بأكملها بتنسيق CSV باستخدام ميزة التصدير.</span><span class="sxs-lookup"><span data-stu-id="3ca23-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="3ca23-120">لمزيد من المعلومات، راجع [التحقق من حالة صحة المستشعر في Microsoft Defender لنقطة النهاية](/microsoft-365/security/defender-endpoint/check-sensor-status).</span><span class="sxs-lookup"><span data-stu-id="3ca23-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="3ca23-121">لمزيد من المعلومات حول سبب عدم تنشيط الجهاز أو تكوينه بشكل خاطئ، راجع إصلاح أدوات الاستشعار غير الصحية في [Microsoft Defender لنقطة النهاية](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span><span class="sxs-lookup"><span data-stu-id="3ca23-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
