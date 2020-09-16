---
title: داتابروتيكتيون-Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731226"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="d52d4-102">تمكين تشفير Bitlocker باستخدام Intune</span><span class="sxs-lookup"><span data-stu-id="d52d4-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="d52d4-103">يمكن استخدام نهج حماية نقطه نهاية Intune لتكوين إعدادات تشفير Bitlocker لأجهزه Windows.</span><span class="sxs-lookup"><span data-stu-id="d52d4-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="d52d4-104">لمزيد من المعلومات ، راجع [إعدادات Windows 10 (والإصدارات الأحدث) لحماية الاجهزه باستخدام Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="d52d4-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="d52d4-105">يجب ان تكون علي علم بان العديد من الاجهزه الجديدة التي تقوم بتشغيل Windows 10 تدعم تشفير Bitlocker التلقائي ، الذي يتم تشغيله بدون تطبيق نهج MDM.</span><span class="sxs-lookup"><span data-stu-id="d52d4-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="d52d4-106">قد يؤثر هذا علي تطبيق النهج في حال تم تكوين الإعدادات غير الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="d52d4-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="d52d4-107">راجع الاسئله المتداولة التالية لمزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="d52d4-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="d52d4-108">للحصول علي معلومات حول استكشاف أخطاء bitlocker وإصلاحها ، راجع [استكشاف أخطاء نهج bitlocker وإصلاحها في Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="d52d4-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="d52d4-109">**الأسئلة المتداولة**</span><span class="sxs-lookup"><span data-stu-id="d52d4-109">**FAQ**</span></span>

 <span data-ttu-id="d52d4-110">س: ما هي إصدارات تشفير أجهزه دعم Windows التي تستخدم نهج حماية نقطه النهاية ؟</span><span class="sxs-lookup"><span data-stu-id="d52d4-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="d52d4-111">ج: يتم تطبيق الإعدادات الموجودة في نهج حماية نقطه نهاية Intune باستخدام [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="d52d4-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="d52d4-112">لا تدعم كل إصدارات Windows أو إصداراتها التي تعتمد Bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="d52d4-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="d52d4-113">في الوقت الحالي ، يتم دعم إصدارات Windows التالية: Enterprise و التعليم والهاتف المحمول والمؤسسة المحمولة والاحترافية (الإصدار 1809 والإصدارات الأحدث).</span><span class="sxs-lookup"><span data-stu-id="d52d4-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="d52d4-114">س: إذا تم تشفير جهاز بالفعل بواسطة Bitlocker باستخدام الإعدادات الافتراضية لنظام التشغيل التلقائي لأسلوب التشفير وقوه التشفير (128 إكستس) ، سيتم تطبيق نهج باستخدام إعدادات مختلفه تلقائيا بتشغيل الإعدادات الجديدة ؟</span><span class="sxs-lookup"><span data-stu-id="d52d4-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="d52d4-115">ج: لا.</span><span class="sxs-lookup"><span data-stu-id="d52d4-115">A: No.</span></span> <span data-ttu-id="d52d4-116">لتطبيق إعدادات التشفير الجديدة ، يجب فك تشفير محرك الاقراص أولا.</span><span class="sxs-lookup"><span data-stu-id="d52d4-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="d52d4-117">**ملاحظه:** بالنسبة إلى الاجهزه التي يتم تسجيلها باستخدام Autopilot ، لا يتم تشغيل التشفير التلقائي الذي سيحدث اثناء OOBE حتى يتم تقييم نهج Intune ، مما يسمح باستخدام الإعدادات المستندة إلى النهج في مكان الافتراضيات لنظام التشغيل.</span><span class="sxs-lookup"><span data-stu-id="d52d4-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="d52d4-118">س: إذا تم تشفير جهاز كنتيجة لتطبيق النهج Intune ، فهل سيتم فك تشفيره عند أزاله هذا النهج ؟</span><span class="sxs-lookup"><span data-stu-id="d52d4-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="d52d4-119">ج: لا تؤدي أزاله النهج المرتبط بالتشفير إلى فك تشفير محركات الاقراص التي تم تكوينها.</span><span class="sxs-lookup"><span data-stu-id="d52d4-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="d52d4-120">س: لماذا يعرض نهج التوافق ل Intune عدم تمكين Bitlocker لجهازي ، علي الرغم من انه ؟</span><span class="sxs-lookup"><span data-stu-id="d52d4-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="d52d4-121">ج: يستخدم الاعداد "تم تمكين Bitlocker" في نهج التوافق في Intune لعميل مصادقه الحماية الخاصة بجهاز Windows (دها).</span><span class="sxs-lookup"><span data-stu-id="d52d4-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="d52d4-122">يقيس هذا العميل حاله الجهاز فقط في وقت التمهيد.</span><span class="sxs-lookup"><span data-stu-id="d52d4-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="d52d4-123">إذا لم يتم أعاده تشغيل جهاز منذ اكتمال تشفير Bitlocker ، فلن تقوم خدمه عميل دها بالإبلاغ عن Bitlocker كما هو نشط.</span><span class="sxs-lookup"><span data-stu-id="d52d4-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 