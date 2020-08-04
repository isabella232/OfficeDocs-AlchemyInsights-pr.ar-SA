---
title: مشكلات متعلقة بشبكة VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554711"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="a0809-102">مشكلات متعلقة بشبكة VPN</span><span class="sxs-lookup"><span data-stu-id="a0809-102">VPN related issues</span></span>

<span data-ttu-id="a0809-103">يعتمد التنفيذ الناجح لاتصال VPN لعملاء MDM على ملف تعريف تم نشره يعكس متطلبات البنية التحتية لـ VPN بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="a0809-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="a0809-104">للحصول على الإعدادات المناسبة للأنظمة الأساسية العميل الذي تقوم بالتحقق منها، راجع:</span><span class="sxs-lookup"><span data-stu-id="a0809-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="a0809-105">إعدادات الجهاز ثلاثي الأبعاد ويندوز ويندوز 10 لإضافة اتصالات VPN باستخدام Intune</span><span class="sxs-lookup"><span data-stu-id="a0809-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="a0809-106">إضافة إعدادات VPN على أجهزة iOS وiPadOS في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a0809-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="a0809-107">إعدادات جهاز أندرويد لتكوين VPN في Intune</span><span class="sxs-lookup"><span data-stu-id="a0809-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="a0809-108">إضافة إعدادات VPN على أجهزة macOS في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a0809-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="a0809-109">إذا كان ملف تعريف VPN يستخدم مصادقة مستندة إلى الشهادة، تأكد من نشر شهادات الجذر و ملفات تعريف شهادة مصادقة العميل المرتبطة بملف تعريف VPN بنجاح.</span><span class="sxs-lookup"><span data-stu-id="a0809-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="a0809-110">**القضايا المشتركة**</span><span class="sxs-lookup"><span data-stu-id="a0809-110">**Common Issues**</span></span>

<span data-ttu-id="a0809-111">**لقد قمت بنشر ملف تعريف VPN على جهاز. Intune يظهر أنه كان ناجحا، ولكن الجهاز لا يتصل VPN.**</span><span class="sxs-lookup"><span data-stu-id="a0809-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="a0809-112">حالة ناجحة يعني أن Intune نشر التشكيل الجانبي كما تم تكوينها بنجاح.</span><span class="sxs-lookup"><span data-stu-id="a0809-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="a0809-113">ومع ذلك، قد لا تتطابق هذه التكوينات مع متطلبات الشبكة و/أو المصادقة.</span><span class="sxs-lookup"><span data-stu-id="a0809-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="a0809-114">مراجعة سجلات في البنية التحتية وخدمة المصادقة (على ملقم VPN و NPS/ Radius الملقم) للحصول على مزيد من التفاصيل حول الاتصال محاولة.</span><span class="sxs-lookup"><span data-stu-id="a0809-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="a0809-115">قد تحتاج إلى العمل مع فريق البنية الأساسية للشبكة، أو مع مورد VPN التابع لجهة خارجية، لجمع سجلات ومراجعةها.</span><span class="sxs-lookup"><span data-stu-id="a0809-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="a0809-116">**عند تكوين VPN مخصص لنظام iOS، لا يتم توفير ميزة الشبكة الافتراضية الخاصة لكل تطبيق.**</span><span class="sxs-lookup"><span data-stu-id="a0809-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="a0809-117">تتوفر حاليًا شبكة VPN لكل تطبيق لأجهزة iOS في Intune لقائمة محددة من مقدمي الخدمات والشركاء ، الذين يجب عليهم أيضًا تلبية متطلبات الشهادة قبل تكوين VPN لكل تطبيق.</span><span class="sxs-lookup"><span data-stu-id="a0809-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="a0809-118">لمزيد من المعلومات، راجع [إعداد الشبكة الافتراضية الخاصة (VPN) لكل تطبيق لأجهزة iOS/iPadOS في Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="a0809-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="a0809-119">لمزيد من المعلومات حول كافة أنواع اتصالات VPN في Intune، راجع [إنشاء ملفات تعريف VPN للاتصال بخوادم VPN في Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="a0809-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="a0809-120">**لا يتم تشغيل iOS عند الطلب VPN عند الوصول إلى مجال مكون**</span><span class="sxs-lookup"><span data-stu-id="a0809-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="a0809-121">لاختبار إعدادات VPN التلقائية، قم بتعيين القيم التالية:</span><span class="sxs-lookup"><span data-stu-id="a0809-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="a0809-122">أريد القيام بما يلي: **تقييم كل محاولة اتصال**</span><span class="sxs-lookup"><span data-stu-id="a0809-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="a0809-123">اختر ما إذا كنت تريد الاتصال: **الاتصال إذا لزم الأمر**</span><span class="sxs-lookup"><span data-stu-id="a0809-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="a0809-124">عندما يقوم المستخدمون بالوصول إلى هذه المجالات: *اسم المجال* **الهدف**</span><span class="sxs-lookup"><span data-stu-id="a0809-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="a0809-125">إذا كان التكوين أعلاه غير ناجح، أضف العنصر التالي:</span><span class="sxs-lookup"><span data-stu-id="a0809-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="a0809-126">عندما يكون URL هذا غير قابل للوصول، قوة الاتصال VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="a0809-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>