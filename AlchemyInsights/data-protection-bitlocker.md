---
title: DataProtection-Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908697"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="e9f81-102">تمكين تشفير Bitlocker باستخدام اينتوني</span><span class="sxs-lookup"><span data-stu-id="e9f81-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="e9f81-103">يمكن استخدام نهج حماية نقطه النهاية اينتوني لتكوين إعدادات تشفير Bitlocker لأجهزه Windows.</span><span class="sxs-lookup"><span data-stu-id="e9f81-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="e9f81-104">لمزيد من المعلومات ، راجع [إعدادات Windows 10 (والإصدارات الأحدث) لحماية الاجهزه باستخدام اينتوني](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="e9f81-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="e9f81-105">يجب ان تدرك ان العديد من الاجهزه الأحدث التي تعمل بنظام التشغيل Windows 10 تدعم تشفير Bitlocker التلقائي ، والذي يتم تشغيله بدون تطبيق نهج MDM.</span><span class="sxs-lookup"><span data-stu-id="e9f81-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="e9f81-106">قد يؤثر هذا علي تطبيق النهج إذا تم تكوين الإعدادات غير الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="e9f81-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="e9f81-107">راجع الاسئله الشائعة التالية لمزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="e9f81-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="e9f81-108">للحصول علي معلومات حول استكشاف مشكلات bitlocker وإصلاحها ، راجع [استكشاف أخطاء نهج bitlocker وإصلاحها في Microsoft اينتوني](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="e9f81-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="e9f81-109">**الأسئلة المتداولة**</span><span class="sxs-lookup"><span data-stu-id="e9f81-109">**FAQ**</span></span>

 <span data-ttu-id="e9f81-110">س: اي إصدارات من Windows دعم تشفير الجهاز باستخدام "نهج حماية نقطه النهاية" ؟</span><span class="sxs-lookup"><span data-stu-id="e9f81-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="e9f81-111">A: يتم تطبيق الإعدادات في نهج حماية نقطه النهاية اينتوني باستخدام [CSP Bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="e9f81-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="e9f81-112">لا تدعم كافة الإصدارات أو البنيات من Windows CSP Bitlocker.</span><span class="sxs-lookup"><span data-stu-id="e9f81-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="e9f81-113">في هذا الوقت ، يتم اعتماد إصدارات Windows التالية: المؤسسة ، التعليم ، الجوال ، المؤسسات المتنقلة ، والمهنية (بناء 1809 والإصدارات الأحدث).</span><span class="sxs-lookup"><span data-stu-id="e9f81-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="e9f81-114">س: إذا كان الجهاز مشفرا بالفعل مع Bitlocker باستخدام الإعدادات الافتراضية لنظام التشغيل لأسلوب التشفير وقوه التشفير (اكستس-AES-128) ، فان تطبيق نهج بإعدادات مختلفه يؤدي تلقائيا إلى أعاده تشفير محرك الاقراص مع الإعدادات الجديدة ؟</span><span class="sxs-lookup"><span data-stu-id="e9f81-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="e9f81-115">A: لا.</span><span class="sxs-lookup"><span data-stu-id="e9f81-115">A: No.</span></span> <span data-ttu-id="e9f81-116">لتطبيق إعدادات التشفير الجديدة ، يجب أولا فك تشفير محرك الاقراص.</span><span class="sxs-lookup"><span data-stu-id="e9f81-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="e9f81-117">**ملاحظه:** بالنسبة للاجهزه التي يتم تسجيلها مع الطيار الألى ، لا يتم تشغيل التشفير التلقائي الذي قد يحدث اثناء OOBE حتى يتم تقييم نهج اينتوني ، والذي يسمح باستخدام الإعدادات المستندة إلى النهج بدلا من افتراضيات نظام التشغيل.</span><span class="sxs-lookup"><span data-stu-id="e9f81-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="e9f81-118">س: إذا تم تشفير جهاز كنتيجة لتطبيق نهج اينتوني ، سيتم فك تشفير عند أزاله هذا النهج ؟</span><span class="sxs-lookup"><span data-stu-id="e9f81-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="e9f81-119">A: أزاله النهج المتعلقة بالتشفير لا ينتج عن فك تشفير محركات الاقراص التي تم تكوينها.</span><span class="sxs-lookup"><span data-stu-id="e9f81-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="e9f81-120">س: لماذا تظهر "سياسة التوافق اينتوني" ان جهازي لم يتم تمكين Bitlocker ، حتى ولو كان ؟</span><span class="sxs-lookup"><span data-stu-id="e9f81-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="e9f81-121">A: يستخدم الاعداد "تمكين Bitlocker" في نهج التوافق اينتوني عميل مصادقه صحة جهاز Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="e9f81-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="e9f81-122">يقيس هذا العميل فقط حاله الجهاز في وقت التمهيد.</span><span class="sxs-lookup"><span data-stu-id="e9f81-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="e9f81-123">لذلك إذا لم يتم أعاده تمهيد الجهاز منذ اكتمال تشفير Bitlocker ، لن تقوم خدمه العميل DHA بالإبلاغ عن Bitlocker علي انه نشط.</span><span class="sxs-lookup"><span data-stu-id="e9f81-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 