---
title: استكشاف مشكله برت وإصلاحها
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573291"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="7e1bb-102">استكشاف مشكله برت وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="7e1bb-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="7e1bb-103">لكي تكتمل عمليه المصادقة علي اي جهاز ، يجب ان يكون مسجلا بالبالكامل وفي حاله جيده ويمكنه الحصول علي رمز تحديث أساسي (برت).</span><span class="sxs-lookup"><span data-stu-id="7e1bb-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="7e1bb-104">تحتاج عمليه التسجيل المختلط في Azure AD join إلى الاجهزه التي يجب ان تكون علي شبكه الشركة.</span><span class="sxs-lookup"><span data-stu-id="7e1bb-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="7e1bb-105">كما يعمل أيضا عبر الشبكات الظاهرية ، ولكن هناك بعض الكافياتس.</span><span class="sxs-lookup"><span data-stu-id="7e1bb-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="7e1bb-106">لقد سمعنا العملاء الذين يحتاجون إلى مساعده في استكشاف عمليه التسجيل المختلطة في Azure AD join وإصلاحها ببموجب ظروف العمل عن بعد.</span><span class="sxs-lookup"><span data-stu-id="7e1bb-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="7e1bb-107">اليك تصنيف تفصيلي لما يحدث "ضمن غطاء" اثناء عمليه التسجيل.</span><span class="sxs-lookup"><span data-stu-id="7e1bb-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="7e1bb-108">**بيئة المصادقة السحابية (باستخدام المزامنة الخاصة بتجزئه كلمه مرور Azure AD أو المصادقة التمريري)**</span><span class="sxs-lookup"><span data-stu-id="7e1bb-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="7e1bb-109">يعرف تدفق التسجيل هذا أيضا "الصلة بالمزامنة".</span><span class="sxs-lookup"><span data-stu-id="7e1bb-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="7e1bb-110">يكتشف Windows 10 سجل سكب عند تسجيل دخول المستخدم إلى الجهاز.</span><span class="sxs-lookup"><span data-stu-id="7e1bb-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="7e1bb-111">يحاول الجهاز أولا استرداد معلومات المستاجر من جانب العميل سكب في التسجيل [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="7e1bb-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="7e1bb-112">لمزيد من المعلومات ، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="7e1bb-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="7e1bb-113">إذا فشلت هذه العملية ، سيتصل الجهاز بخدمه Active Directory المحلية (AD) للحصول علي معلومات المستاجر من نقطه اتصال الخدمة (سكب).</span><span class="sxs-lookup"><span data-stu-id="7e1bb-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="7e1bb-114">للتحقق من السكب ، يرجى الرجوع إلى هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="7e1bb-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="7e1bb-115">نوصي بتمكين سكب في الإعلان واستخدام سكب من جانب العميل للتحقق من صحة مبدئي.</span><span class="sxs-lookup"><span data-stu-id="7e1bb-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="7e1bb-116">يحاول نظام التشغيل Windows 10 التواصل مع Azure AD تحت سياق النظام للمصادقة علي نفسه مقابل Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7e1bb-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="7e1bb-117">يمكنك التحقق مما إذا كان بإمكان الجهاز الوصول إلى موارد Microsoft ضمن حساب النظام باستخدام البرنامج النصي لاتصال تسجيل جهاز الاختبار.</span><span class="sxs-lookup"><span data-stu-id="7e1bb-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="7e1bb-118">ينشئ Windows 10 شهادة موقعه ذاتيا ويخزنها ضمن كائن الكمبيوتر في الإعلان المحلي.</span><span class="sxs-lookup"><span data-stu-id="7e1bb-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="7e1bb-119">يتطلب ذلك ان يتم الاطلاع علي الخطوط الخاصة بالمجال.</span><span class="sxs-lookup"><span data-stu-id="7e1bb-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="7e1bb-120">تتم مزامنة كائن الجهاز الذي تمت الشهادة معه في Azure AD عبر Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="7e1bb-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="7e1bb-121">دوره المزامنة كل 30 دقيقه بشكل افتراضي ، ولكنها تعتمد علي تكوين Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="7e1bb-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="7e1bb-122">لمزيد من المعلومات ، يرجى الرجوع إلى هذا [المستند](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="7e1bb-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="7e1bb-123">في هذه المرحلة ، يجب ان تكون قادرا علي رؤية جهاز الموضوع في الحالة "معلق" ضمن "الجهاز النصليه في Azure Portal".</span><span class="sxs-lookup"><span data-stu-id="7e1bb-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="7e1bb-124">عند تسجيل دخول المستخدم التالي إلى Windows 10 ، سيتم إكمال التسجيل.</span><span class="sxs-lookup"><span data-stu-id="7e1bb-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="7e1bb-125">إذا كنت تستخدم VPN وكانت عمليه تسجيل الدخول إلى التسجيل الخاص بك تقوم بإنهاء اتصال المجال ، فيمكنك تشغيل التسجيل يدويا:</span><span class="sxs-lookup"><span data-stu-id="7e1bb-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="7e1bb-126">إصدار دسريجكمد/join محليا في مطالبه المسؤول أو عن بعد عبر بسيكسيك إلى الكمبيوتر الشخصي.</span><span class="sxs-lookup"><span data-stu-id="7e1bb-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="7e1bb-127">علي سبيل المثال ، بسيكسيك \\ win10client01 cmd ، دسريجكمد/الصلة</span><span class="sxs-lookup"><span data-stu-id="7e1bb-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="7e1bb-128">للحصول علي مزيد من التفاصيل حول مشاكل الصلة المختلطة ، راجع [مشكله استكشاف الأخطاء وإصلاحها](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="7e1bb-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
