---
title: المصطلحات المفقودة من SharePoint علي الإنترنت مخزن الأجل
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053500"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="a834f-102">تمكين تشفير Bitlocker باستخدام اينتوني</span><span class="sxs-lookup"><span data-stu-id="a834f-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="a834f-103">يمكن استخدام نهج حماية نقطه النهاية اينتوني لتكوين إعدادات التشفير Boitlocker لأجهزه Windows كما هو موضح في: Windows10 (والإصدارات الأحدث) لحماية الاجهزه باستخدام اينتوني</span><span class="sxs-lookup"><span data-stu-id="a834f-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="a834f-104">يجب ان تدرك ان العديد من الاجهزه الأحدث التي تعمل بنظام التشغيل Windows 10 تدعم تشفير bitlocker التلقائي الذي يتم تشغيله بدون تطبيق نهج MDM.</span><span class="sxs-lookup"><span data-stu-id="a834f-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="a834f-105">قد يؤثر هذا علي تطبيق النهج إذا تم تكوين الإعدادات غير الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="a834f-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="a834f-106">راجع الاسئله الشائعة لمزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="a834f-106">See FAQ for more detail.</span></span>


<span data-ttu-id="a834f-107">اسئله  وأجوبه Q: اي إصدارات من Windows دعم تشفير الجهاز باستخدام "نهج حماية نقطه النهاية" ؟</span><span class="sxs-lookup"><span data-stu-id="a834f-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="a834f-108"> A: يتم تطبيق الإعدادات في نهج حماية نقطه النهاية اينتوني باستخدام CSP Bitlocker.</span><span class="sxs-lookup"><span data-stu-id="a834f-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="a834f-109">لا تدعم كافة الإصدارات ولا البنيات من Windows CSP Bitlocker. 
     </span><span class="sxs-lookup"><span data-stu-id="a834f-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="a834f-110">في هذا الوقت إصدارات ويندوز: المؤسسة; يتم دعم التعليم والمحمول والمؤسسات المتنقلة والمهنية (من بناء 1809 فصاعدا).</span><span class="sxs-lookup"><span data-stu-id="a834f-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="a834f-111">Q: إذا تم تشفير جهاز بالفعل مع Bitlocker باستخدام الإعدادات الافتراضية لنظام التشغيل لأسلوب التشفير وقوه التشفير (اكستس-AES-128) سيتم تطبيق نهج مع إعدادات مختلفه تلقائيا بتشغيل أعاده تشفير محرك الاقراص مع الإعدادات الجديدة ؟</span><span class="sxs-lookup"><span data-stu-id="a834f-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="a834f-112">A: لا.</span><span class="sxs-lookup"><span data-stu-id="a834f-112">A: No.</span></span> <span data-ttu-id="a834f-113">من أجل تطبيق إعدادات التشفير الجديدة يجب أولا فك تشفير محرك الاقراص.</span><span class="sxs-lookup"><span data-stu-id="a834f-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="a834f-114">ملاحظه للاجهزه التي يتم تسجيلها مع الطيار الألى التشفير التلقائي التي قد تحدث اثناء OOBE لا يتم تشغيله حتى يتم تقييم نهج اينتوني الذي يسمح الإعدادات المستندة إلى نهج ليتم استخدامها بدلا من الافتراضيات نظام التشغيل</span><span class="sxs-lookup"><span data-stu-id="a834f-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="a834f-115">س إذا تم تشفير جهاز نتيجة تطبيق نهج اينتوني سيتم فك تشفير عند أزاله هذا النهج ؟</span><span class="sxs-lookup"><span data-stu-id="a834f-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="a834f-116">A: لا يؤدي أزاله النهج المرتبط بالتشفير إلى فك تشفير محركات الاقراص التي تم تكوينها.</span><span class="sxs-lookup"><span data-stu-id="a834f-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="a834f-117">س: لماذا يظهر نهج التوافق اينتوني ان جهازي ليس لديه "تمكين Bitlocker" ولكن هو ؟</span><span class="sxs-lookup"><span data-stu-id="a834f-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="a834f-118">A: يستخدم الاعداد "تمكين Bitlocker" في نهج التوافق اينتوني عميل مصادقه صحة جهاز Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="a834f-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="a834f-119">يقيس هذا العميل فقط حاله الجهاز في وقت التمهيد.</span><span class="sxs-lookup"><span data-stu-id="a834f-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="a834f-120">حتى إذا لم يتم أعاده تمهيد الجهاز منذ اكتمال تشفير bitlocker خدمه العميل DHA لن تقرير bitlocker بأنها نشطه.</span><span class="sxs-lookup"><span data-stu-id="a834f-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>