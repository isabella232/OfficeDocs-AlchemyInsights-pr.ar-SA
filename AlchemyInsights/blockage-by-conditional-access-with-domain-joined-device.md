---
title: يتم حظري بواسطة "الوصول الشرطي" مع جهاز انضم إلى المجال
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/20/2021
ms.locfileid: "51034869"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="027b4-102">يتم حظري بواسطة "الوصول الشرطي" مع جهاز انضم إلى المجال</span><span class="sxs-lookup"><span data-stu-id="027b4-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="027b4-103">**أدوات موصى بها بشدة**</span><span class="sxs-lookup"><span data-stu-id="027b4-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="027b4-104">أداة م استكشاف [الأخطاء وإصلاحها](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) لتسجيل الجهاز - الأداة التي تساعد في استكشاف مشاكل تسجيل الجهاز الأكثر شيوعا وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="027b4-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="027b4-105">[اختبار البرنامج النصي لاتصال](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) تسجيل الجهاز - البرنامج النصي الذي يساعد على ضمان وصول الجهاز إلى نقاط نهاية تسجيل الجهاز ضمن حساب النظام.</span><span class="sxs-lookup"><span data-stu-id="027b4-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="027b4-106">[برنامج نصي لتنظيف جهاز Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) - البرنامج النصي الذي يمكنك من البحث عن الأجهزة التي لم يتم انتهاءها وإدارتها في بيئتك.</span><span class="sxs-lookup"><span data-stu-id="027b4-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="027b4-107">فيما يلي بعض الأسباب الشائعة وراء فشل الوصول الشرطي لجهاز انضم إلى مجال (Azure AD المختلط).</span><span class="sxs-lookup"><span data-stu-id="027b4-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="027b4-108">**لا يوجد Azure AD PRT** على الجهاز - يجب التأكد من أن الجهاز لديه رمز التحديث الأساسي ل Azure AD Token (PRT).</span><span class="sxs-lookup"><span data-stu-id="027b4-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="027b4-109">لمزيد من المعلومات حول PRT، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="027b4-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="027b4-110">للتحقق مما إذا كان لديك Azure AD PRT، يمكنك تشغيل الأمر على الجهاز والتحقق مما إذا كانت `dsregcmd/status` "AzureAdPrt" تساوي "YES".</span><span class="sxs-lookup"><span data-stu-id="027b4-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="027b4-111">إذا كانت "AzureAdPrt" "NO"، فتحقق مما يلي:</span><span class="sxs-lookup"><span data-stu-id="027b4-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="027b4-112">سواء كان لديك بيئة مضمنة مع **AD FS،** ولا يمكن الوصول إليها من الشبكات المنزلية الخاصة بالمستخدمين : في هذه الحالة، تأكد من إمكانية الوصول إلى نقاط النهاية "اسم المستخدم" من إكسترانت.</span><span class="sxs-lookup"><span data-stu-id="027b4-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="027b4-113">إذا كان AD FS الخاص بك خلف VPN، فتأكد من اتصال المستخدمين ب VPN ثم إعادة تسجيل الدخول إلى الجهاز.</span><span class="sxs-lookup"><span data-stu-id="027b4-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="027b4-114">لمزيد من المعلومات، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="027b4-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="027b4-115">**ما إذا كانت TPM** في الجهاز بها أخطاء وبالتالي يتعذر عليها مصادقة الجهاز : تحقق من "tpm.msc" لمعرفة ما إذا كانت حالة TPM هي "جاهز".</span><span class="sxs-lookup"><span data-stu-id="027b4-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="027b4-116">إذا لم يكن الأمر كذلك، فدير الجهاز `dsregcmd/leave` واتركه ينضم مرة أخرى إلى Azure AD.</span><span class="sxs-lookup"><span data-stu-id="027b4-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="027b4-117">بعد ذلك، حاول مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="027b4-117">Then, try again.</span></span> <span data-ttu-id="027b4-118">لمزيد من المعلومات، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="027b4-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="027b4-119">**أنت تستخدم موفر هوية** جهة خارجية، لا يدعم WS-Trust.</span><span class="sxs-lookup"><span data-stu-id="027b4-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="027b4-120">كما هو موضح في مستنداتنا، لا يمكن للأجهزة المختلطة المنضمة إلى Azure AD العمل في هذه الحالة.</span><span class="sxs-lookup"><span data-stu-id="027b4-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="027b4-121">الرجاء العمل مع موفر الهوية للحصول على الدعم.</span><span class="sxs-lookup"><span data-stu-id="027b4-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="027b4-122">يستخدم المستخدمون مستعرض Chrome بدون حسابات **Windows 10** أو ملحق Office لا يستخدم Chrome تلقائيا PRT على الأجهزة المنضمة إلى AAD أو المختلطة المنضمة إلى **AAD**: يؤدي ذلك إلى فشل أي من سياسات الوصول الشرطي المستندة إلى الجهاز، مع عرض رسالة الخطأ "جهاز غير مسجل".</span><span class="sxs-lookup"><span data-stu-id="027b4-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="027b4-123">لاستخدام مستعرض Chrome بشكل صحيح، يجب تثبيت "حسابات Windows 10" أو "ملحق Office إلى مستعرض Chrome الخاص المستخدمين" عبر SCCM أو Intune.</span><span class="sxs-lookup"><span data-stu-id="027b4-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="027b4-124">لمزيد من المعلومات، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="027b4-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="027b4-125">إذا لم يكن من الممكن دفع الملحق عن بعد، قم بإعلام المستخدمين بتثبيت أحد الملحقات أعلاه يدويا للوصول إلى التطبيقات خلف الوصول الشرطي المستند إلى الجهاز.</span><span class="sxs-lookup"><span data-stu-id="027b4-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="027b4-126">لمزيد من المعلومات، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="027b4-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="027b4-127">كان الجهاز مختلطا بشكل صحيح انضم **Azure AD،** ولكن تم حذفه أو تعطيله عن طريق الخطأ، إما بسبب مزامنة التغييرات في Azure AD Connect أو من مدخل Azure : إذا حدث ذلك، لن يتم التعرف على كائن الجهاز على أنه جهاز منضم بالكامل على الرغم من أن حالة "AzureAdJoined" و"PRT" تظهر ك صالحة على الجهاز.</span><span class="sxs-lookup"><span data-stu-id="027b4-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="027b4-128">لإصلاح هذه المشكلة، يمكنك التشغيل على الأجهزة المتأثرة واتركها تنضم مجددا إلى `dsregcmd/leave` Azure AD.</span><span class="sxs-lookup"><span data-stu-id="027b4-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="027b4-129">لمزيد من المعلومات، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="027b4-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="027b4-130">إذا كانت أجهزتك تعمل على تحديث Windows 10، 1809، باستخدام VPN/وكيل السحابة وشاهدت مشاكل تتعلق ب "AzureAdPrt" (AzureAdPrt) أو أي تطبيق به مشكلة في SSO (outlook لا يتصل علبة البريد على الرغم من وجود PRT لديك)، فتأكد من وجود هذا التصحيح [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) أو التحديث التراكمي ل [أبريل KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) لمنع حالات فشل PRT على هذه الأجهزة.</span><span class="sxs-lookup"><span data-stu-id="027b4-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















