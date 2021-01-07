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
ms.openlocfilehash: 482c08b31e4d97ca5cc9ec6e35e309cb7536036d
ms.sourcegitcommit: 58ac31a58c956a4d74f66bd4151a2311dc361b78
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/07/2021
ms.locfileid: "49778180"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="d1a85-102">تمكين تشفير Bitlocker باستخدام Intune</span><span class="sxs-lookup"><span data-stu-id="d1a85-102">Enabling Bitlocker encryption with Intune</span></span>

<span data-ttu-id="d1a85-103">يمكن استخدام نهج حماية نقطه نهاية Intune لتكوين إعدادات تشفير Bitlocker لأجهزه Windows.</span><span class="sxs-lookup"><span data-stu-id="d1a85-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="d1a85-104">لمزيد من المعلومات ، راجع [إعدادات Windows 10 (والإصدارات الأحدث) لحماية الاجهزه باستخدام Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="d1a85-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>

<span data-ttu-id="d1a85-105">بالاضافه إلى نهج حماية نقطه النهاية ، يوجد أيضا تقرير تشفير يوفر طريقه عرض أكثر تفصيلا لحاله التشفير للاجهزه.</span><span class="sxs-lookup"><span data-stu-id="d1a85-105">In addition to the Endpoint Protection Policy there is also an Encryption Report which provides a more detailed view of the encryption status for devices.</span></span> <span data-ttu-id="d1a85-106">يمكن الوصول إلى هذا التقرير من مدخل ميم ضمن **ال> أجهزه التي تعرض جهاز العرض**، ثم ضمن **التكوين** تحديد [تقرير التشفير](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).</span><span class="sxs-lookup"><span data-stu-id="d1a85-106">This report can be accessed from the MEM portal under **Devices > Monitor**, and then under **Configuration** select [Encryption report](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).</span></span>

<span data-ttu-id="d1a85-107">إذا اكتشفت انه سيفشل تمكين Bitlocker بالشكل المتوقع أو إذا كان ملف التعريف الذي يتم استخدامه لتمكين Bitlocker في حاله خطا ، فالرجاء مراجعه تقرير التشفير للحصول علي فهم أفضل لسبب حدوث السلوك.</span><span class="sxs-lookup"><span data-stu-id="d1a85-107">If you find that Bitlocker fails to be enabled as expected or that the profile being used to enable Bitlocker is in an error state, please review the encryption report to get a better understanding of why the behavior is occurring.</span></span>

<span data-ttu-id="d1a85-108">للبحث عن تفاصيل حول كيفيه تفسير التقرير بما في ذلك قيم حاله التشفير المختلفة ، راجع [تشفير جهاز المراقبة باستخدام Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).</span><span class="sxs-lookup"><span data-stu-id="d1a85-108">To find details on how to interpret the report including the various encryption status values, see [Monitor device encryption with Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).</span></span>

<span data-ttu-id="d1a85-109">يجب ان تكون علي علم بان العديد من الاجهزه الجديدة التي تقوم بتشغيل Windows 10 تدعم تشفير Bitlocker التلقائي ، الذي يتم تشغيله بدون تطبيق نهج MDM.</span><span class="sxs-lookup"><span data-stu-id="d1a85-109">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="d1a85-110">قد يؤثر هذا علي تطبيق النهج في حال تم تكوين الإعدادات غير الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="d1a85-110">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="d1a85-111">راجع الاسئله المتداولة التالية لمزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="d1a85-111">See the following FAQ for more detail.</span></span>

<span data-ttu-id="d1a85-112">للحصول علي معلومات حول استكشاف أخطاء bitlocker وإصلاحها ، راجع [استكشاف أخطاء نهج bitlocker وإصلاحها في Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="d1a85-112">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="d1a85-113">**الأسئلة المتداولة**</span><span class="sxs-lookup"><span data-stu-id="d1a85-113">**FAQ**</span></span>

<span data-ttu-id="d1a85-114">س: ما هي إصدارات تشفير أجهزه دعم Windows التي تستخدم نهج حماية نقطه النهاية ؟</span><span class="sxs-lookup"><span data-stu-id="d1a85-114">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="d1a85-115">ج: يتم تطبيق الإعدادات الموجودة في نهج حماية نقطه نهاية Intune باستخدام [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="d1a85-115">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="d1a85-116">لا تدعم كل إصدارات Windows أو إصداراتها التي تعتمد Bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="d1a85-116">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="d1a85-117">س: كيف يمكن تمكين Bitlocker علي الاجهزه من دون الحاجة إلى تفاعل المستخدم النهائي ؟</span><span class="sxs-lookup"><span data-stu-id="d1a85-117">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="d1a85-118">ج: طالما كانت المتطلبات الضرورية للإصدارات السابقة ممكنة لتمكين Bitlocker "التشفير التلقائي" عبر Intune.</span><span class="sxs-lookup"><span data-stu-id="d1a85-118">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="d1a85-119">راجع تفاصيل متطلبات الجهاز وإعدادات النهج المثال لتمكين التشفير الصامت في المستند التالي: [يمكنك تمكين تشفير Bitlocker بدون مطالبه](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="d1a85-119">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="d1a85-120">س: إذا تم تشفير جهاز بالفعل بواسطة Bitlocker باستخدام الإعدادات الافتراضية لنظام التشغيل التلقائي لأسلوب التشفير وقوه التشفير (128 إكستس) ، سيتم تطبيق نهج باستخدام إعدادات مختلفه تلقائيا بتشغيل الإعدادات الجديدة ؟</span><span class="sxs-lookup"><span data-stu-id="d1a85-120">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="d1a85-121">ج: لا.</span><span class="sxs-lookup"><span data-stu-id="d1a85-121">A: No.</span></span> <span data-ttu-id="d1a85-122">لتطبيق إعدادات التشفير الجديدة ، يجب فك تشفير محرك الاقراص أولا.</span><span class="sxs-lookup"><span data-stu-id="d1a85-122">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="d1a85-123">**ملاحظه:** بالنسبة إلى الاجهزه التي يتم تسجيلها باستخدام Autopilot ، لا يتم تشغيل التشفير التلقائي الذي سيحدث اثناء OOBE حتى يتم تقييم نهج Intune ، مما يسمح باستخدام الإعدادات المستندة إلى النهج في مكان الافتراضيات لنظام التشغيل.</span><span class="sxs-lookup"><span data-stu-id="d1a85-123">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="d1a85-124">س: إذا تم تشفير جهاز كنتيجة لتطبيق النهج Intune ، فهل سيتم فك تشفيره عند أزاله هذا النهج ؟</span><span class="sxs-lookup"><span data-stu-id="d1a85-124">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="d1a85-125">ج: لا تؤدي أزاله النهج المرتبط بالتشفير إلى فك تشفير محركات الاقراص التي تم تكوينها.</span><span class="sxs-lookup"><span data-stu-id="d1a85-125">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="d1a85-126">س: لماذا يعرض نهج التوافق ل Intune عدم تمكين Bitlocker لجهازي ، علي الرغم من انه ؟</span><span class="sxs-lookup"><span data-stu-id="d1a85-126">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="d1a85-127">ج: يستخدم الاعداد "تم تمكين Bitlocker" في نهج التوافق في Intune لعميل مصادقه الحماية الخاصة بجهاز Windows (دا).</span><span class="sxs-lookup"><span data-stu-id="d1a85-127">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="d1a85-128">يقيس هذا العميل حاله الجهاز فقط في وقت التمهيد.</span><span class="sxs-lookup"><span data-stu-id="d1a85-128">This client only measures device state at boot time.</span></span> <span data-ttu-id="d1a85-129">إذا لم يتم أعاده تشغيل جهاز منذ اكتمال تشفير Bitlocker ، فلن تقوم خدمه عميل دا بالإبلاغ عن Bitlocker كما هو نشط.</span><span class="sxs-lookup"><span data-stu-id="d1a85-129">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 