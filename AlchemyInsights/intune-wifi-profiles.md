---
title: ملفات تعريف Intune Wi-fi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696248"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="53473-102">ملفات تعريف Intune Wi-fi</span><span class="sxs-lookup"><span data-stu-id="53473-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="53473-103">يعتمد التنفيذ الناجح لاتصال Wi-fi لعملاء MDM علي ملف تعريف موزع بشكل صحيح يعكس متطلبات البنية الاساسيه للشركات Wi-fi.</span><span class="sxs-lookup"><span data-stu-id="53473-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="53473-104">لمراجعه الإعدادات المناسبة للانظمه الاساسيه التي تقوم بالتحقق منها ، راجع:</span><span class="sxs-lookup"><span data-stu-id="53473-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="53473-105">أضافه إعدادات Wi-fi للاجهزه التي تعمل بنظام التشغيل Android في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="53473-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="53473-106">أضافه إعدادات Wi-fi للاجهزه التي تعمل بنظام Android Enterprise المخصصة والاجهزه المدارة بالبالكامل في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="53473-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="53473-107">أضافه إعدادات Wi-fi للاجهزه التي تعمل بنظام التشغيل iOS و إيبادوس في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="53473-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="53473-108">أضافه إعدادات Wi-fi لنظام التشغيل Windows 10 والاجهزه الأحدث في Intune</span><span class="sxs-lookup"><span data-stu-id="53473-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="53473-109">استيراد إعدادات Wi-fi لأجهزه Windows في Intune</span><span class="sxs-lookup"><span data-stu-id="53473-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="53473-110">**المشاكل الشائعة**</span><span class="sxs-lookup"><span data-stu-id="53473-110">**Common Issues**</span></span>

<span data-ttu-id="53473-111">**أقوم بنشر ملف تعريف Wi-fi المعتمد علي شهادة منشوره محدده في ملف تعريف Wi-fi. ومع ذلك ، تعرض ملفات تعريف التكوين حاله خطا.**</span><span class="sxs-lookup"><span data-stu-id="53473-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="53473-112">تاكد من ان جهازك استلم الشهادة.</span><span class="sxs-lookup"><span data-stu-id="53473-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="53473-113">في Intune ، انتقل إلى **كل الاجهزه** وحدد **تكوين جهاز**> الجهاز.</span><span class="sxs-lookup"><span data-stu-id="53473-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="53473-114">تاكد من ان كل ملفات التعريف المتوقعة مدرجه وفي حاله ناجحه.</span><span class="sxs-lookup"><span data-stu-id="53473-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="53473-115">بالنسبة إلى ملف تعريف Android ، إذا كان لديك شهادات متوسطه في سلسله الشهادات ، فتاكد من نشرها علي أجهزه Android.</span><span class="sxs-lookup"><span data-stu-id="53473-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="53473-116">للتحقق من حاله الشهادة ، انتقل إلى ملفات تعريف **تكوين الجهاز**الخاصة  >  **Profiles**  >  **Android intermediate CA**  >  **Properties**  >  **بالشهادات الموثوق بها**لنظام التشغيل Android وسيطه.</span><span class="sxs-lookup"><span data-stu-id="53473-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="53473-117">إذا استمر ظهور الأخطاء ، فراجع القسمين الإجراءات واستكشاف الأخطاء وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="53473-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="53473-118">لمزيد من المعلومات ، راجع [نظره عامه حول استكشاف أخطاء ملفات تعريف شهادات سسيب وإصلاحها باستخدام Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="53473-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="53473-119">**لقد قمت بنشر ملف تعريف Wi-fi إلى جهاز. يعرض Intune انه نجح ، ولكن الجهاز لا يتصل بشبكه Wi-fi.**</span><span class="sxs-lookup"><span data-stu-id="53473-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="53473-120">تعني الحالة ناجح ان يقوم Intune بنشر ملف التعريف كما تم تكوينه بنجاح.</span><span class="sxs-lookup"><span data-stu-id="53473-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="53473-121">ومع ذلك ، قد لا تتطابق هذه التكوينات مع متطلبات الشبكة و/أو المصادقة.</span><span class="sxs-lookup"><span data-stu-id="53473-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="53473-122">للحصول علي مزيد من التفاصيل حول الاتصال الذي تمت محاولته ، راجع السجلات في البنية الاساسيه وخدمه المصادقة (علي جهاز التحكم بنقطه وصول wi-fi وخادم NPS/Radius).</span><span class="sxs-lookup"><span data-stu-id="53473-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="53473-123">قد يتعين عليك استخدام فريق البنية الاساسيه للشبكة ، أو مورد Wi-fi للجهة الخارجية ، لجمع السجلات ومراجعتها.</span><span class="sxs-lookup"><span data-stu-id="53473-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>