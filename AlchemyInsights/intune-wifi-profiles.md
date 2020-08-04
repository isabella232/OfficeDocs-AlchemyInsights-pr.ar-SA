---
title: ملفات تعريف Wi-Fi Intune
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554720"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="076d0-102">ملفات تعريف Wi-Fi Intune</span><span class="sxs-lookup"><span data-stu-id="076d0-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="076d0-103">يعتمد التنفيذ الناجح لاتصال Wi-Fi لعملاء MDM على ملف تعريف تم نشره بشكل صحيح يعكس متطلبات البنية الأساسية للواي فاي للشركات.</span><span class="sxs-lookup"><span data-stu-id="076d0-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="076d0-104">لمراجعة الإعدادات المناسبة للأنظمة الأساسية العميلة التي تقوم بالتحقق منها، راجع:</span><span class="sxs-lookup"><span data-stu-id="076d0-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="076d0-105">إضافة إعدادات Wi-Fi للأجهزة التي تعمل بنظام التشغيل Android في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="076d0-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="076d0-106">إضافة إعدادات Wi-Fi لأجهزة Android Enterprise المخصصة والمدارة بالكامل في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="076d0-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="076d0-107">إضافة إعدادات Wi-Fi لأجهزة iOS وiPadOS في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="076d0-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="076d0-108">إضافة إعدادات Wi-Fi لـ Windows 10 والأجهزة الأحدث في Intune</span><span class="sxs-lookup"><span data-stu-id="076d0-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="076d0-109">استيراد إعدادات Wi-Fi لأجهزة Windows في Intune</span><span class="sxs-lookup"><span data-stu-id="076d0-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="076d0-110">**القضايا المشتركة**</span><span class="sxs-lookup"><span data-stu-id="076d0-110">**Common Issues**</span></span>

<span data-ttu-id="076d0-111">**أقوم بنشر ملف تعريف Wi-Fi يعتمد على شهادة منشورة محددة في ملف تعريف Wi-Fi. ومع ذلك، تظهر ملفات تعريف التكوين حالة خطأ.**</span><span class="sxs-lookup"><span data-stu-id="076d0-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="076d0-112">تحقق من أن الجهاز قد تلقى الشهادة.</span><span class="sxs-lookup"><span data-stu-id="076d0-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="076d0-113">في Intune، انتقل إلى **كافة الأجهزة** وحدد الجهاز > **تكوين الجهاز**.</span><span class="sxs-lookup"><span data-stu-id="076d0-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="076d0-114">تحقق من أن كافة التشكيلات الجانبية المتوقعة مدرجة وفي حالة ناجحة.</span><span class="sxs-lookup"><span data-stu-id="076d0-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="076d0-115">بالنسبة لملف تعريف Android، إذا كان لديك شهادات متوسطة في سلسلة الشهادات، تأكد من نشرها على أجهزة Android.</span><span class="sxs-lookup"><span data-stu-id="076d0-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="076d0-116">للتحقق من حالة الشهادة، انتقل إلى التشكيلات الجانبية لتكوين **الجهاز**  >  **Profiles**  >  **Android متوسطة CA**  >  **Properties**Certificate  >  **موثوق .**</span><span class="sxs-lookup"><span data-stu-id="076d0-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="076d0-117">إذا استمر عرض الأخطاء، راجع الإجراءات وأقسام استكشاف الأخطاء وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="076d0-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="076d0-118">لمزيد من المعلومات، راجع [نظرة عامة لاستكشاف أخطاء ملفات تعريف شهادات SCEP مع Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="076d0-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="076d0-119">**قمت بنشر ملف تعريف Wi-Fi على جهاز. Intune هو تبين أنه كان ناجحا، ولكن الجهاز لا يتصل واي فاي.**</span><span class="sxs-lookup"><span data-stu-id="076d0-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="076d0-120">حالة ناجحة يعني أن Intune نشر التشكيل الجانبي كما تم تكوينها بنجاح.</span><span class="sxs-lookup"><span data-stu-id="076d0-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="076d0-121">ومع ذلك، قد لا تتطابق هذه التكوينات مع متطلبات الشبكة و/أو المصادقة.</span><span class="sxs-lookup"><span data-stu-id="076d0-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="076d0-122">لمزيد من التفاصيل حول الاتصال الذي تمت محاولة الاتصال به، قم بمراجعة سجلات في البنية التحتية وخدمة المصادقة (على وحدة تحكم نقطة وصول Wi-Fi وخادم NPS/Radius).</span><span class="sxs-lookup"><span data-stu-id="076d0-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="076d0-123">قد تحتاج إلى العمل مع فريق البنية الأساسية للشبكة، أو مع مورد Wi-Fi التابع لجهة خارجية، لجمع سجلات ومراجعةها.</span><span class="sxs-lookup"><span data-stu-id="076d0-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>