---
title: يتم حظري بواسطة "الوصول الشرطي" مع جهاز متوافق
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034775"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a><span data-ttu-id="71e2c-102">يتم حظري بواسطة "الوصول الشرطي" مع جهاز متوافق</span><span class="sxs-lookup"><span data-stu-id="71e2c-102">I’m getting blocked by Conditional Access with compliant device</span></span>

<span data-ttu-id="71e2c-103">**أدوات موصى بها بشدة**</span><span class="sxs-lookup"><span data-stu-id="71e2c-103">**Highly Recommended Tools**</span></span>

- <span data-ttu-id="71e2c-104">أداة م استكشاف [الأخطاء وإصلاحها](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) لتسجيل الجهاز - أداة شاملة تساعد على استكشاف مشاكل تسجيل الأجهزة الأكثر شيوعا وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="71e2c-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - A comprehensive tool that helps troubleshoot the most common device registration issues.</span></span>
- <span data-ttu-id="71e2c-105">[اختبار البرنامج النصي لاتصال](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) تسجيل الجهاز - أداة تستخدم للتأكد من أن الجهاز يمكنه الوصول إلى نقاط نهاية تسجيل الجهاز ضمن حساب النظام.</span><span class="sxs-lookup"><span data-stu-id="71e2c-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - A tool used to ensure that a device can access Device Registration endpoints under the system account.</span></span>
- <span data-ttu-id="71e2c-106">[برنامج نصي لتنظيف جهاز Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) - أداة تستخدم للبحث عن الأجهزة التي لا تعمل بشكل جيد وإدارتها في بيئتك.</span><span class="sxs-lookup"><span data-stu-id="71e2c-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - A tool used to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="71e2c-107">فيما يلي بعض الأسباب الشائعة لفشل الوصول الشرطي لجهاز متوافق أو  سبب تلقي المستخدمين لرسالة لا يمكنك الوصول إليها من هنا أثناء طلب تسجيل الدخول إلى مورد المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="71e2c-107">Here are some common reasons why Conditional Access may be failing for a compliant device or why your users may be receiving **You can't get there from here** message during a sign-in request to an organizational resource.</span></span>

1. <span data-ttu-id="71e2c-108">**الجهاز غير في حالة جهاز مطلوب مع MDM:**</span><span class="sxs-lookup"><span data-stu-id="71e2c-108">**Device is not in a required device state with an MDM**:</span></span>

<span data-ttu-id="71e2c-109">تحقق من أن الجهاز مسجل مع موفر MDM معتمد مثل Intune وضع *علامة عليه كمتوافق.*</span><span class="sxs-lookup"><span data-stu-id="71e2c-109">Validate that the device is enrolled with an approved MDM provider like Intune and *marked as compliant*.</span></span> <span data-ttu-id="71e2c-110">لمزيد من المعلومات حول Intune، راجع هذا [المستند](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment).</span><span class="sxs-lookup"><span data-stu-id="71e2c-110">For more information on Intune see this [document](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment).</span></span> <span data-ttu-id="71e2c-111">للحصول على فهم أفضل لتوافق الأجهزة و Intune، راجع استخدام نهج التوافق لتعيين قواعد للأجهزة التي [تديرها باستخدام Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started).</span><span class="sxs-lookup"><span data-stu-id="71e2c-111">For better understanding of device compliance and Intune, see [use compliance policy to set rules for devices you manage with Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started).</span></span> <span data-ttu-id="71e2c-112">إذا كنت تواجه مشاكل في تسجيل جهاز باستخدام Intune، فاعثر على تفاصيل استكشاف الأخطاء وإصلاحها في تسجيل الجهاز وإصلاحها [في Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="71e2c-112">If you are having issues enrolling a device with Intune, find troubleshooting details at [Troubleshoot device enrollment in Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span> <span data-ttu-id="71e2c-113">لمزيد من دعم Intune، قم بإنشاء طلب دعم.</span><span class="sxs-lookup"><span data-stu-id="71e2c-113">For further Intune support, create a support request.</span></span> <span data-ttu-id="71e2c-114">للقيام بذلك، تفضل بزيارة [صفحة تعليمات ودعم Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).</span><span class="sxs-lookup"><span data-stu-id="71e2c-114">To do so, visit the [Intune Help and Support page](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).</span></span>

2. <span data-ttu-id="71e2c-115">**الجهاز غير منضم إلى شبكة المؤسسات**:</span><span class="sxs-lookup"><span data-stu-id="71e2c-115">**Device is not joined to the organizations network**:</span></span>

<span data-ttu-id="71e2c-116">للوصول إلى موارد المؤسسة، يجب أن يكون الجهاز متصلا بشبكة المؤسسة، إما من خلال اتصال مباشر أو شبكة ظاهرية خاصة (VPN)، وأن يكون متصلا أيضا ب Azure Active Directory أو المحلي.</span><span class="sxs-lookup"><span data-stu-id="71e2c-116">For access to organizational resources, the device has to be connected to the organization's network, either through direct connection or a virtual private network (VPN), and also joined to on-premise or Azure Active Directory.</span></span> <span data-ttu-id="71e2c-117">للانضمام إلى جهاز عمل إلى شبكة المؤسسة، راجع الانضمام إلى جهاز العمل إلى [شبكة مؤسستك](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network).</span><span class="sxs-lookup"><span data-stu-id="71e2c-117">To join a work device to the organization network, see [Join your work device to your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network).</span></span> <span data-ttu-id="71e2c-118">لتسجيل جهاز شخصي/BYOD، راجع تسجيل جهازك [الشخصي على شبكة مؤسستك](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).</span><span class="sxs-lookup"><span data-stu-id="71e2c-118">To register a personal/BYOD device, see [Register your personal device on your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).</span></span>

- <span data-ttu-id="71e2c-119">للتحقق مما إذا كان الجهاز قد انضم إلى الشبكة، [](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) يمكنك اتباع الخطوات الخاصة بالأجهزة المسجلة هنا أو أجهزة العمل [هنا.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined)</span><span class="sxs-lookup"><span data-stu-id="71e2c-119">To validate whether the device has joined the network, you can follow the steps for registered devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) or work devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined).</span></span> <span data-ttu-id="71e2c-120">لنطاق المشكلة إلى اتصال شبكة المؤسسة، اتبع الإرشادات أدناه:</span><span class="sxs-lookup"><span data-stu-id="71e2c-120">To scope the issue to Org network connectivity, follow guidelines below:</span></span>

    1. <span data-ttu-id="71e2c-121">سجل الدخول إلى Windows باستخدام حساب العمل أو المدرسة، على سبيل المثال، alain@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="71e2c-121">Sign in to Windows using your work or school account,  for example, alain@contoso.com.</span></span>
    2. <span data-ttu-id="71e2c-122">اتصل بشبكة مؤسستك من خلال VPN أو DirectAccesss.</span><span class="sxs-lookup"><span data-stu-id="71e2c-122">Connect to your organization's network through a VPN or DirectAccess.</span></span>
    3. <span data-ttu-id="71e2c-123">بعد الاتصال، اضغط على مفتاح **شعار Windows+L** لقفل جهازك.</span><span class="sxs-lookup"><span data-stu-id="71e2c-123">After you're connected, press the **Windows logo key+L** to lock your device.</span></span>
    4. <span data-ttu-id="71e2c-124">قم بإلغاء تأمين جهازك باستخدام حساب العمل أو المدرسة، ثم حاول الوصول إلى التطبيق أو الخدمة التي تسبب مشاكل مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="71e2c-124">Unlock your device using your work or school account, and then try to access the problematic app or service again.</span></span>

<span data-ttu-id="71e2c-125">إذا رأيت رسالة الخطأ **لا** يمكنك الوصول إلى هناك من هنا مرة أخرى، فمن المرجح أن تكون المشكلة في مكان آخر.</span><span class="sxs-lookup"><span data-stu-id="71e2c-125">If you see the **You can't get there from here** error message again, issue is likely elsewhere.</span></span>

3. <span data-ttu-id="71e2c-126">**نظام التشغيل غير معتمد:**</span><span class="sxs-lookup"><span data-stu-id="71e2c-126">**Operating system is not supported**:</span></span>

<span data-ttu-id="71e2c-127">تأكد من تشغيل إصدار معتمد من نظام التشغيل، بما في ذلك:</span><span class="sxs-lookup"><span data-stu-id="71e2c-127">Ensure that you're running a supported version of the operating system, including:</span></span>

- <span data-ttu-id="71e2c-128">**عميل Windows**: Windows 7 أو أي وقت لاحق</span><span class="sxs-lookup"><span data-stu-id="71e2c-128">**Windows Client**: Windows 7 or later</span></span>

- <span data-ttu-id="71e2c-129">**Windows Server**: Windows Server 2008 R2 أو أي وقت لاحق</span><span class="sxs-lookup"><span data-stu-id="71e2c-129">**Windows Server**: Windows Server 2008 R2 or later</span></span>

- <span data-ttu-id="71e2c-130">**macOS**: macOS X أو أي وقت لاحق</span><span class="sxs-lookup"><span data-stu-id="71e2c-130">**macOS**: macOS X or later</span></span>

- <span data-ttu-id="71e2c-131">**Android و iOS**: أحدث إصدار من أنظمة تشغيل الأجهزة المحمولة التي تعمل بنظامي التشغيل Android و iOS</span><span class="sxs-lookup"><span data-stu-id="71e2c-131">**Android and iOS**: Latest version of Android and iOS mobile operating systems</span></span>

4. <span data-ttu-id="71e2c-132">**مستعرض ويب غير معتمد:**</span><span class="sxs-lookup"><span data-stu-id="71e2c-132">**Web browser is not supported**:</span></span>

<span data-ttu-id="71e2c-133">الرجاء العثور على المستعرضات المعتمدة أدناه.</span><span class="sxs-lookup"><span data-stu-id="71e2c-133">Please find supported browsers below.</span></span> <span data-ttu-id="71e2c-134">بالنسبة إلى دعم Chrome مع Windows 1703 أو الإصدارات الأحدث، يجب استخدام ملحق حسابات Windows 10.</span><span class="sxs-lookup"><span data-stu-id="71e2c-134">For Chrome support with Windows 1703 or later versions, a Windows 10 Accounts extension is required.</span></span> <span data-ttu-id="71e2c-135">بالنسبة إلى Edge 85+، يحتاج المستخدم إلى تسجيل الدخول لتمرير معلومات توافق الجهاز بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="71e2c-135">For Edge 85+, the user needs to be signed in to properly pass device compliance information.</span></span> <span data-ttu-id="71e2c-136">لمزيد من التفاصيل، راجع [هنا](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="71e2c-136">For more details, see [here](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

- <span data-ttu-id="71e2c-137">**Windows 10**: Microsoft Edge، Internet Explorer، Chrome</span><span class="sxs-lookup"><span data-stu-id="71e2c-137">**Windows 10**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="71e2c-138">**Windows 8 / 8.1**: Internet Explorer، Chrome</span><span class="sxs-lookup"><span data-stu-id="71e2c-138">**Windows 8 / 8.1**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="71e2c-139">**Windows 7**: Internet Explorer، Chrome</span><span class="sxs-lookup"><span data-stu-id="71e2c-139">**Windows 7**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="71e2c-140">**iOS**: Microsoft Edge، مستعرض Intune المدار، Safari</span><span class="sxs-lookup"><span data-stu-id="71e2c-140">**iOS**: Microsoft Edge, Intune Managed Browser, Safari</span></span>
- <span data-ttu-id="71e2c-141">**Android**: **Microsoft Edge**: مستعرض Intune المدار، Chrome</span><span class="sxs-lookup"><span data-stu-id="71e2c-141">**Android**: **Microsoft Edge**: Intune Managed Browser, Chrome</span></span>
- <span data-ttu-id="71e2c-142">**Windows Phone**: Microsoft Edge، Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="71e2c-142">**Windows Phone**: Microsoft Edge, Internet Explorer</span></span>
- <span data-ttu-id="71e2c-143">**Windows Server 2019**: Microsoft Edge، Internet Explorer، Chrome</span><span class="sxs-lookup"><span data-stu-id="71e2c-143">**Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="71e2c-144">**Windows Server 2016**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="71e2c-144">**Windows Server 2016**: Internet Explorer</span></span>
- <span data-ttu-id="71e2c-145">**Windows Server 2012 R2**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="71e2c-145">**Windows Server 2012 R2**: Internet Explorer</span></span>
- <span data-ttu-id="71e2c-146">**Windows Server 2008 R2**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="71e2c-146">**Windows Server 2008 R2**: Internet Explorer</span></span>
- <span data-ttu-id="71e2c-147">**macOS**: Chrome، Safari</span><span class="sxs-lookup"><span data-stu-id="71e2c-147">**macOS**: Chrome, Safari</span></span>

<span data-ttu-id="71e2c-148">يمكنك العثور على مزيد من المعلومات حول **الرسالة** لا يمكنك الوصول إلى هناك والخطوات المتعلقة استكشاف الأخطاء وإصلاحها [هنا](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).</span><span class="sxs-lookup"><span data-stu-id="71e2c-148">Find more information on the **You can't get there** message and troubleshooting steps [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).</span></span>
