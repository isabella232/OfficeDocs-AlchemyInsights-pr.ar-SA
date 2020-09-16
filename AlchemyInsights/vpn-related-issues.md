---
title: المشاكل ذات الصلة ب VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726078"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="bb607-102">المشاكل ذات الصلة ب VPN</span><span class="sxs-lookup"><span data-stu-id="bb607-102">VPN related issues</span></span>

<span data-ttu-id="bb607-103">يعتمد التنفيذ الناجح لاتصال VPN لعملاء MDM علي ملف تعريف منشور يعكس بشكل صحيح متطلبات البنية الاساسيه ل VPN.</span><span class="sxs-lookup"><span data-stu-id="bb607-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="bb607-104">للحصول علي الإعدادات المناسبة للانظمه العميلة التي تقوم بالتحقق منها ، راجع:</span><span class="sxs-lookup"><span data-stu-id="bb607-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="bb607-105">إعدادات جهاز windows 10 و Windows هولوجرافيك لأضافه اتصالات VPN باستخدام Intune</span><span class="sxs-lookup"><span data-stu-id="bb607-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="bb607-106">أضافه إعدادات VPN علي أجهزه iOS و إيبادوس في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bb607-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="bb607-107">إعدادات جهاز Android لتكوين VPN في Intune</span><span class="sxs-lookup"><span data-stu-id="bb607-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="bb607-108">أضافه إعدادات VPN علي أجهزه macOS في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bb607-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="bb607-109">إذا كان ملف تعريف VPN الخاص بك يستخدم مصادقه مستنده إلى الشهادة ، فتاكد من ان الشهادة الجذر وملفات تعريف شهادة مصادقه العميل المرتبطة بملف تعريف VPN تم نشرها بنجاح.</span><span class="sxs-lookup"><span data-stu-id="bb607-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="bb607-110">**المشاكل الشائعة**</span><span class="sxs-lookup"><span data-stu-id="bb607-110">**Common Issues**</span></span>

<span data-ttu-id="bb607-111">**لقد قمت بنشر ملف تعريف VPN إلى جهاز. يعرض Intune انه نجح ، ولكن الجهاز لا يتصل بشبكه VPN.**</span><span class="sxs-lookup"><span data-stu-id="bb607-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="bb607-112">تعني الحالة ناجح ان يقوم Intune بنشر ملف التعريف كما تم تكوينه بنجاح.</span><span class="sxs-lookup"><span data-stu-id="bb607-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="bb607-113">ومع ذلك ، قد لا تتطابق هذه التكوينات مع متطلبات الشبكة و/أو المصادقة.</span><span class="sxs-lookup"><span data-stu-id="bb607-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="bb607-114">راجع السجلات في البنية الاساسيه وخدمه المصادقة (علي خادم VPN وخادم NPS/Radius) للحصول علي مزيد من التفاصيل حول الاتصال الذي تمت محاولته.</span><span class="sxs-lookup"><span data-stu-id="bb607-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="bb607-115">قد تحتاج إلى العمل علي فريق البنية الاساسيه للشبكة ، أو مورد VPN التابع لجهة خارجيه ، لجمع السجلات ومراجعتها.</span><span class="sxs-lookup"><span data-stu-id="bb607-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="bb607-116">**عندما أقوم بتكوين VPN مخصص لنظام التشغيل iOS ، لم يتم توفير ميزه الإصدار VPN لكل تطبيق.**</span><span class="sxs-lookup"><span data-stu-id="bb607-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="bb607-117">يتوفر حاليا لكل تطبيق للاجهزه التي تعمل بنظام التشغيل iOS في Intune لقائمه معينه من الموفرين والشركاء ، الذين يجب أيضا ان يلبيوا متطلبات الشهادة قبل تكوين VPN لكل تطبيق.</span><span class="sxs-lookup"><span data-stu-id="bb607-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="bb607-118">للحصول علي مزيد من المعلومات ، راجع اعداد [شبكه الاتصال الظاهرية الخاصة بكل تطبيق (VPN) لأجهزه iOS/إيبادوس في Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="bb607-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="bb607-119">للحصول علي مزيد من المعلومات حول كل أنواع اتصالات VPN في Intune ، راجع [إنشاء ملفات تعريف VPN للاتصال بخوادم VPN في intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="bb607-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="bb607-120">**لا يتم تشغيل iOS عند الطلب في الشبكة**</span><span class="sxs-lookup"><span data-stu-id="bb607-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="bb607-121">لاختبار إعدادات VPN التلقائية ، قم بتعيين القيم التالية:</span><span class="sxs-lookup"><span data-stu-id="bb607-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="bb607-122">أريد القيام بما يلي: **تقييم كل محاولة اتصال**</span><span class="sxs-lookup"><span data-stu-id="bb607-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="bb607-123">اختيار ما إذا كنت تريد الاتصال: **الاتصال عند الحاجة**</span><span class="sxs-lookup"><span data-stu-id="bb607-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="bb607-124">عندما يصل المستخدمون إلى هذه المجالات: *اسم المجال* **الهدف**</span><span class="sxs-lookup"><span data-stu-id="bb607-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="bb607-125">إذا لم ينجح التكوين أعلاه ، فأضف العنصر التالي:</span><span class="sxs-lookup"><span data-stu-id="bb607-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="bb607-126">عند تعذر الوصول إلى عنوان URL هذا ، قم بفرض توصيل VPN: **بادورل**</span><span class="sxs-lookup"><span data-stu-id="bb607-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>