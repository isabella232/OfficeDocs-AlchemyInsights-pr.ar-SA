---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 8166a055d7a967faab83484619b443cc98239c7c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815602"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="961b0-102">تمكين تشفير Bitlocker باستخدام Intune</span><span class="sxs-lookup"><span data-stu-id="961b0-102">Enabling Bitlocker encryption with Intune</span></span>

<span data-ttu-id="961b0-103">يمكن استخدام نهج حماية نقطة نهاية Intune لتكوين إعدادات تشفير Bitlocker للأجهزة التي تعمل بنظام Windows.</span><span class="sxs-lookup"><span data-stu-id="961b0-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="961b0-104">لمزيد من المعلومات، راجع [إعدادات Windows 10 (واللاحقة) لحماية الأجهزة باستخدام Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="961b0-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>

<span data-ttu-id="961b0-105">بالإضافة إلى نهج حماية نقطة النهاية، يوجد أيضا تقرير تشفير يوفر طريقة عرض أكثر تفصيلا حول حالة التشفير للأجهزة.</span><span class="sxs-lookup"><span data-stu-id="961b0-105">In addition to the Endpoint Protection Policy there is also an Encryption Report which provides a more detailed view of the encryption status for devices.</span></span> <span data-ttu-id="961b0-106">يمكن الوصول إلى هذا التقرير من مدخل MEM ضمن الأجهزة > **جهاز العرض**، ثم ضمن تكوين **حدد** [تقرير التشفير](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).</span><span class="sxs-lookup"><span data-stu-id="961b0-106">This report can be accessed from the MEM portal under **Devices > Monitor**, and then under **Configuration** select [Encryption report](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).</span></span>

<span data-ttu-id="961b0-107">إذا لم يتم تمكين Bitlocker كما هو متوقع أو إذا كان ملف التعريف المستخدم لتمكين Bitlocker في حالة خطأ، فيرجى مراجعة تقرير التشفير للحصول على فهم أفضل لل سبب حدوث السلوك.</span><span class="sxs-lookup"><span data-stu-id="961b0-107">If you find that Bitlocker fails to be enabled as expected or that the profile being used to enable Bitlocker is in an error state, please review the encryption report to get a better understanding of why the behavior is occurring.</span></span>

<span data-ttu-id="961b0-108">للعثور على تفاصيل حول كيفية تفسير التقرير بما في ذلك قيم حالة التشفير المختلفة، راجع مراقبة تشفير الأجهزة [باستخدام Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).</span><span class="sxs-lookup"><span data-stu-id="961b0-108">To find details on how to interpret the report including the various encryption status values, see [Monitor device encryption with Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).</span></span>

<span data-ttu-id="961b0-109">يجب أن تدرك أن العديد من الأجهزة الجديدة التي تعمل بنظام التشغيل Windows 10 تدعم تشفير Bitlocker التلقائي، الذي يتم تشغيله بدون تطبيق نهج MDM.</span><span class="sxs-lookup"><span data-stu-id="961b0-109">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="961b0-110">قد يؤثر ذلك على تطبيق النهج إذا تم تكوين إعدادات غير افتراضية.</span><span class="sxs-lookup"><span data-stu-id="961b0-110">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="961b0-111">راجع الأسئلة الشائعة التالية للحصول على مزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="961b0-111">See the following FAQ for more detail.</span></span>

<span data-ttu-id="961b0-112">للحصول على معلومات حول استكشاف مشاكل bitlocker وإصلاحها، راجع استكشاف مشاكل سياسات BitLocker وإصلاحها [في Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="961b0-112">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="961b0-113">**الأسئلة المتداولة**</span><span class="sxs-lookup"><span data-stu-id="961b0-113">**FAQ**</span></span>

<span data-ttu-id="961b0-114">س: ما هي إصدارات تشفير الأجهزة التي تدعم Windows باستخدام نهج حماية نقطة النهاية؟</span><span class="sxs-lookup"><span data-stu-id="961b0-114">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="961b0-115">ج: يتم تنفيذ الإعدادات في نهج حماية نقطة نهاية Intune باستخدام [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="961b0-115">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="961b0-116">لا تدعم كل إصدارات أو إصدارات Windows Bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="961b0-116">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="961b0-117">س: كيف يمكن تمكين Bitlocker على الأجهزة دون الحاجة إلى تفاعل المستخدم النهائي؟</span><span class="sxs-lookup"><span data-stu-id="961b0-117">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="961b0-118">ج: طالما تم تحقيق المتطلبات الأساسية الضرورية، فمن الممكن تمكين Bitlocker "التشفير الصامت" من خلال Intune.</span><span class="sxs-lookup"><span data-stu-id="961b0-118">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="961b0-119">راجع تفاصيل متطلبات الجهاز وإعدادات النهج على سبيل المثال لتمكين التشفير الصامت في المستعرض التالي: تمكين تشفير [Bitlocker بصمت](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="961b0-119">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="961b0-120">س: إذا كان الجهاز مشفرا بالفعل باستخدام Bitlocker باستخدام إعدادات نظام التشغيل الافتراضية لطريقة التشفير وقوة التشفير (XTS-AES-128)، فهل سيتم تطبيق نهج بإعدادات مختلفة تلقائيا على إعادة تشفير محرك الأقراص باستخدام الإعدادات الجديدة؟</span><span class="sxs-lookup"><span data-stu-id="961b0-120">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="961b0-121">ج: لا.</span><span class="sxs-lookup"><span data-stu-id="961b0-121">A: No.</span></span> <span data-ttu-id="961b0-122">لتطبيق إعدادات التشفير الجديدة، يجب أولا فك تشفير محرك الأقراص.</span><span class="sxs-lookup"><span data-stu-id="961b0-122">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="961b0-123">**ملاحظة:** بالنسبة للأجهزة التي يتم تسجيلها باستخدام Autopilot، لا يتم تشغيل التشفير التلقائي الذي سيحدث أثناء OOBE حتى يتم تقييم نهج Intune، مما يسمح باستخدام الإعدادات المستندة إلى النهج في مكان الإعدادات الافتراضية ل OS.</span><span class="sxs-lookup"><span data-stu-id="961b0-123">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="961b0-124">س: إذا تم تشفير جهاز نتيجة لتطبيق نهج Intune، فهل سيتم فك تشفيره عند إزالة هذا النهج؟</span><span class="sxs-lookup"><span data-stu-id="961b0-124">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="961b0-125">أ: لا تؤدي إزالة النهج المرتبط بالتشفير إلى فك تشفير محركات الأقراص التي تم تكوينها.</span><span class="sxs-lookup"><span data-stu-id="961b0-125">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="961b0-126">س: لماذا يظهر نهج التوافق في Intune أن جهازي لا يقوم بتمكين Bitlocker، على الرغم من أنه تم تمكينه؟</span><span class="sxs-lookup"><span data-stu-id="961b0-126">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="961b0-127">ج: يستخدم الإعداد "تمكين Bitlocker" في نهج التوافق في Intune عميل التحقق من صحة جهاز Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="961b0-127">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="961b0-128">يقيس هذا العميل حالة الجهاز فقط في وقت التشغيل.</span><span class="sxs-lookup"><span data-stu-id="961b0-128">This client only measures device state at boot time.</span></span> <span data-ttu-id="961b0-129">وبالتالي، إذا لم يتم إعادة تشغيل الجهاز منذ اكتمال تشفير Bitlocker، لن تقوم خدمة عميل DHA ب الإبلاغ عن Bitlocker على أنه نشط.</span><span class="sxs-lookup"><span data-stu-id="961b0-129">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 