---
title: الجهاز في الحالة "معلق"
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/11/2020
ms.locfileid: "49676805"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="28c90-102">الجهاز في الحالة "معلق"</span><span class="sxs-lookup"><span data-stu-id="28c90-102">Device in pending state</span></span>

<span data-ttu-id="28c90-103">**متطلب**</span><span class="sxs-lookup"><span data-stu-id="28c90-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="28c90-104">إذا كنت تقوم باعداد تسجيلات الاجهزه للمرة الاولي ، فالرجاء التاكد من انك قمت بمراجعه [مقدمه حول أداره الاجهزه في Azure Active directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) التي سترشدك علي كيفيه الحصول علي الاجهزه ضمن عنصر التحكم في azure AD.</span><span class="sxs-lookup"><span data-stu-id="28c90-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="28c90-105">إذا كنت تقوم بتسجيل الاجهزه في Azure AD مباشره وقامت بانتسابها في Intune ، ستحتاج إلى التاكد من انك قمت [بتكوين Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ولديك [الترخيص](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) في المكان أولا.</span><span class="sxs-lookup"><span data-stu-id="28c90-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="28c90-106">تاكد من انك مخول بتنفيذ العمليات في Azure AD والإعلان المحلي.</span><span class="sxs-lookup"><span data-stu-id="28c90-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="28c90-107">يمكن للمسؤول العام فقط في Azure AD أداره إعدادات تسجيلات الاجهزه.</span><span class="sxs-lookup"><span data-stu-id="28c90-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="28c90-108">بالاضافه إلى ذلك ، إذا كنت تقوم باعداد التسجيلات التلقائية في Active Directory المحلي ، ستحتاج إلى ان تكون مسؤولا ل Active directory و AD FS (إذا كان ذلك ممكنا).</span><span class="sxs-lookup"><span data-stu-id="28c90-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="28c90-109">تحتاج عمليه التسجيل المختلط في Azure AD join إلى الاجهزه التي يجب ان تكون علي شبكه الشركة.</span><span class="sxs-lookup"><span data-stu-id="28c90-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="28c90-110">كما يعمل أيضا عبر الشبكات الظاهرية ، ولكن هناك بعض الكافيتس.</span><span class="sxs-lookup"><span data-stu-id="28c90-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="28c90-111">لقد سمعنا العملاء الذين يحتاجون إلى مساعده في استكشاف الأخطاء المختلطة لعمليه التسجيل في Azure AD join ضمن ظروف العمل البعيدة.</span><span class="sxs-lookup"><span data-stu-id="28c90-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="28c90-112">**بيئة المصادقة السحابية (باستخدام المزامنة الخاصة بتجزئه كلمه مرور Azure AD أو المصادقة التمريري)**</span><span class="sxs-lookup"><span data-stu-id="28c90-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="28c90-113">يعرف تدفق التسجيل هذا أيضا "الصلة بالمزامنة".</span><span class="sxs-lookup"><span data-stu-id="28c90-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="28c90-114">فيما يلي تصنيف تفصيلي لما يحدث اثناء عمليه التسجيل:</span><span class="sxs-lookup"><span data-stu-id="28c90-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="28c90-115">سجل نقطه اتصال خدمه اكتشاف Windows 10 (سكب) عندما يقوم المستخدم بتسجيل الدخول إلى الجهاز.</span><span class="sxs-lookup"><span data-stu-id="28c90-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="28c90-116">يحاول الجهاز أولا استرداد معلومات المستاجر من جانب العميل سكب في التسجيل [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="28c90-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="28c90-117">لمزيد من المعلومات ، راجع [المستند](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="28c90-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="28c90-118">إذا فشلت هذه العملية ، سيتصل الجهاز بخدمه Active Directory المحلية للحصول علي معلومات المستاجر من سكب.</span><span class="sxs-lookup"><span data-stu-id="28c90-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="28c90-119">للتحقق من السكب ، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="28c90-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="28c90-120">نوصي بتمكين سكب في Active Directory واستخدام سكب من جانب العميل للتحقق من صحة مبدئي.</span><span class="sxs-lookup"><span data-stu-id="28c90-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="28c90-121">يحاول نظام التشغيل Windows 10 التواصل مع Azure AD تحت سياق النظام للمصادقة علي نفسه مقابل Azure AD.</span><span class="sxs-lookup"><span data-stu-id="28c90-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="28c90-122">يمكنك التحقق مما إذا كان بإمكان الجهاز الوصول إلى موارد Microsoft ضمن حساب النظام باستخدام [البرنامج النصي لاتصال تسجيل جهاز الاختبار](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="28c90-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="28c90-123">يقوم Windows 10 بإنشاء شهادة موقعه ذاتيا وتخزينها ضمن كائن الكمبيوتر في Active Directory المحلي.</span><span class="sxs-lookup"><span data-stu-id="28c90-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="28c90-124">يتطلب ذلك ان يتم الاطلاع علي الخطوط الخاصة بالمجال.</span><span class="sxs-lookup"><span data-stu-id="28c90-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="28c90-125">كائن الجهاز الذي تمت مزامنة الشهادة معه في Azure AD عبر Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="28c90-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="28c90-126">دوره المزامنة كل 30 دقيقه بشكل افتراضي ، ولكنها تعتمد علي تكوين Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="28c90-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="28c90-127">لمزيد من المعلومات ، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="28c90-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="28c90-128">في هذه المرحلة ، يجب ان تكون قادرا علي رؤية جهاز الموضوع في الحالة "**معلق**" ضمن "الجهاز النصليه في Azure Portal".</span><span class="sxs-lookup"><span data-stu-id="28c90-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="28c90-129">عند تسجيل دخول المستخدم التالي إلى Windows 10 ، سيتم إكمال التسجيل.</span><span class="sxs-lookup"><span data-stu-id="28c90-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="28c90-130">إذا كنت تستخدم VPN وقامت بتسجيل الدخول ، سيؤدي ذلك إلى إنهاء اتصال المجال ، يمكنك تشغيل التسجيل يدويا.</span><span class="sxs-lookup"><span data-stu-id="28c90-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="28c90-131">لتنفيذ الإجراءات التالية:</span><span class="sxs-lookup"><span data-stu-id="28c90-131">To do that:</span></span>
    >
    > <span data-ttu-id="28c90-132">`dsregcmd /join`الإصدار المحلي لمطالبه المسؤول أو عن بعد عبر بسيكسيك إلى الكمبيوتر الشخصي.</span><span class="sxs-lookup"><span data-stu-id="28c90-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="28c90-133">على سبيل المثال: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="28c90-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="28c90-134">للاطلاع علي المشاكل الشائعة في تسجيل جهاز Azure Active directory ، راجع [الاسئله المتداولة حول الاجهزه](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="28c90-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
