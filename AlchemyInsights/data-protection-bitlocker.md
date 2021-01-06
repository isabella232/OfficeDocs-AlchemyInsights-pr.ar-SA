---
title: داتابروتيكشن-Bitlocker
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
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768804"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="a4fc8-102">تمكين تشفير Bitlocker باستخدام Intune</span><span class="sxs-lookup"><span data-stu-id="a4fc8-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="a4fc8-103">يمكن استخدام نهج حماية نقطه نهاية Intune لتكوين إعدادات تشفير Bitlocker لأجهزه Windows.</span><span class="sxs-lookup"><span data-stu-id="a4fc8-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="a4fc8-104">لمزيد من المعلومات ، راجع [إعدادات Windows 10 (والإصدارات الأحدث) لحماية الاجهزه باستخدام Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="a4fc8-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="a4fc8-105">يجب ان تكون علي علم بان العديد من الاجهزه الجديدة التي تقوم بتشغيل Windows 10 تدعم تشفير Bitlocker التلقائي ، الذي يتم تشغيله بدون تطبيق نهج MDM.</span><span class="sxs-lookup"><span data-stu-id="a4fc8-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="a4fc8-106">قد يؤثر هذا علي تطبيق النهج في حال تم تكوين الإعدادات غير الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="a4fc8-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="a4fc8-107">راجع الاسئله المتداولة التالية لمزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="a4fc8-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="a4fc8-108">للحصول علي معلومات حول استكشاف أخطاء bitlocker وإصلاحها ، راجع [استكشاف أخطاء نهج bitlocker وإصلاحها في Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="a4fc8-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="a4fc8-109">**الأسئلة المتداولة**</span><span class="sxs-lookup"><span data-stu-id="a4fc8-109">**FAQ**</span></span>

<span data-ttu-id="a4fc8-110">س: ما هي إصدارات تشفير أجهزه دعم Windows التي تستخدم نهج حماية نقطه النهاية ؟</span><span class="sxs-lookup"><span data-stu-id="a4fc8-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="a4fc8-111">ج: يتم تطبيق الإعدادات الموجودة في نهج حماية نقطه نهاية Intune باستخدام [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="a4fc8-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="a4fc8-112">لا تدعم كل إصدارات Windows أو إصداراتها التي تعتمد Bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="a4fc8-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="a4fc8-113">س: كيف يمكن تمكين Bitlocker علي الاجهزه من دون الحاجة إلى تفاعل المستخدم النهائي ؟</span><span class="sxs-lookup"><span data-stu-id="a4fc8-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="a4fc8-114">ج: طالما كانت المتطلبات الضرورية للإصدارات السابقة ممكنة لتمكين Bitlocker "التشفير التلقائي" عبر Intune.</span><span class="sxs-lookup"><span data-stu-id="a4fc8-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="a4fc8-115">راجع تفاصيل متطلبات الجهاز وإعدادات النهج المثال لتمكين التشفير الصامت في المستند التالي: [يمكنك تمكين تشفير Bitlocker بدون مطالبه](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="a4fc8-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="a4fc8-116">س: إذا تم تشفير جهاز بالفعل بواسطة Bitlocker باستخدام الإعدادات الافتراضية لنظام التشغيل التلقائي لأسلوب التشفير وقوه التشفير (128 إكستس) ، سيتم تطبيق نهج باستخدام إعدادات مختلفه تلقائيا بتشغيل الإعدادات الجديدة ؟</span><span class="sxs-lookup"><span data-stu-id="a4fc8-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="a4fc8-117">ج: لا.</span><span class="sxs-lookup"><span data-stu-id="a4fc8-117">A: No.</span></span> <span data-ttu-id="a4fc8-118">لتطبيق إعدادات التشفير الجديدة ، يجب فك تشفير محرك الاقراص أولا.</span><span class="sxs-lookup"><span data-stu-id="a4fc8-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="a4fc8-119">**ملاحظه:** بالنسبة إلى الاجهزه التي يتم تسجيلها باستخدام Autopilot ، لا يتم تشغيل التشفير التلقائي الذي سيحدث اثناء OOBE حتى يتم تقييم نهج Intune ، مما يسمح باستخدام الإعدادات المستندة إلى النهج في مكان الافتراضيات لنظام التشغيل.</span><span class="sxs-lookup"><span data-stu-id="a4fc8-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="a4fc8-120">س: إذا تم تشفير جهاز كنتيجة لتطبيق النهج Intune ، فهل سيتم فك تشفيره عند أزاله هذا النهج ؟</span><span class="sxs-lookup"><span data-stu-id="a4fc8-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="a4fc8-121">ج: لا تؤدي أزاله النهج المرتبط بالتشفير إلى فك تشفير محركات الاقراص التي تم تكوينها.</span><span class="sxs-lookup"><span data-stu-id="a4fc8-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="a4fc8-122">س: لماذا يعرض نهج التوافق ل Intune عدم تمكين Bitlocker لجهازي ، علي الرغم من انه ؟</span><span class="sxs-lookup"><span data-stu-id="a4fc8-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="a4fc8-123">ج: يستخدم الاعداد "تم تمكين Bitlocker" في نهج التوافق في Intune لعميل مصادقه الحماية الخاصة بجهاز Windows (دا).</span><span class="sxs-lookup"><span data-stu-id="a4fc8-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="a4fc8-124">يقيس هذا العميل حاله الجهاز فقط في وقت التمهيد.</span><span class="sxs-lookup"><span data-stu-id="a4fc8-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="a4fc8-125">إذا لم يتم أعاده تشغيل جهاز منذ اكتمال تشفير Bitlocker ، فلن تقوم خدمه عميل دا بالإبلاغ عن Bitlocker كما هو نشط.</span><span class="sxs-lookup"><span data-stu-id="a4fc8-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 