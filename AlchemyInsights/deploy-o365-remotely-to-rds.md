---
title: نشر تطبيقات Microsoft 365 ل enterprise for use المشتركة علي RDS أو الخادم الطرفي أو VDI
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 22ded616e82b2e82023b55a1d3ca6251cfb71712
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745522"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="1b97b-102">نشر تطبيقات Microsoft 365 ل enterprise for use المشتركة علي RDS أو الخادم الطرفي أو VDI</span><span class="sxs-lookup"><span data-stu-id="1b97b-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="1b97b-103">لنشر تطبيقات Microsoft 365 للمؤسسة باستخدام خدمات سطح المكتب البعيد (RDS) ، المعروف سابقا بالخدمات الطرفية:</span><span class="sxs-lookup"><span data-stu-id="1b97b-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="1b97b-104">يجب ان يتوفر لديك خطه Microsoft 365 For Business أو خطه Office 365 التي تتضمن تطبيقات Microsoft 365 ل enterprise ، مثل Office 365 Enterprise E3 أو Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="1b97b-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="1b97b-105">لا تتضمن تطبيقات Microsoft 365 للاعمال وخطط Microsoft 365 Business Premium القياسية تطبيقات Microsoft 365 ل enterprise.</span><span class="sxs-lookup"><span data-stu-id="1b97b-105">The Microsoft 365 Apps for business and Microsoft 365 Business Premium Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="1b97b-106">يجب تمكين [تنشيط الكمبيوتر المشترك](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="1b97b-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="1b97b-107">يمكنك أيضا تنزيل [مساعد الإصلاح والدعم من microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) وتشغيله لتثبيت تطبيقات microsoft 365 ل enterprise في وضع تنشيط الكمبيوتر المشترك.</span><span class="sxs-lookup"><span data-stu-id="1b97b-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="1b97b-108">للحصول علي مزيد من المعلومات حول المتطلبات الاساسيه وإرشادات الاعداد والإرشادات علي التثبيتات المخصصة باستخدام أداه نشر Office ، راجع [نشر تطبيقات Microsoft 365 للمؤسسة باستخدام خدمات سطح المكتب البعيد](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="1b97b-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="1b97b-109">لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشترك:</span><span class="sxs-lookup"><span data-stu-id="1b97b-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="1b97b-110">راجع [استكشاف الأخطاء وإصلاحها في تنشيط الكمبيوتر المشترك لتطبيقات Microsoft 365 ل enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="1b97b-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="1b97b-111">راجع [إعادة تعيين تطبيقات Microsoft 365 لحالة تفعيل المؤسسة](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="1b97b-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="1b97b-112">إذا كنت تريد تثبيت تطبيقات Microsoft 365 ل enterprise علي RDS من Microsoft 365 admin center ، ***الذي يستخدم إعدادات التثبيت الافتراضية***، فاستخدم الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="1b97b-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.    <span data-ttu-id="1b97b-113">التحقق من الاشتراك الذي تملكه.</span><span class="sxs-lookup"><span data-stu-id="1b97b-113">Check what subscription you have.</span></span> <span data-ttu-id="1b97b-114">[تعرف علي كيفيه القيام](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)بذلك.</span><span class="sxs-lookup"><span data-stu-id="1b97b-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.    <span data-ttu-id="1b97b-115">إذا لزم الأمر ، فقم بالتبديل إلى اشتراك مختلف.</span><span class="sxs-lookup"><span data-stu-id="1b97b-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="1b97b-116">[تعرف علي كيفيه القيام](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)بذلك.</span><span class="sxs-lookup"><span data-stu-id="1b97b-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3.    <span data-ttu-id="1b97b-117">إذا كان Office مثبتا بالفعل علي RDS server باستخدام اي اشتراكات Microsoft أخرى ، فقم بازاله تثبيته.</span><span class="sxs-lookup"><span data-stu-id="1b97b-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="1b97b-118">علي سبيل المثال ، بالانتقال إلى **"لوحه التحكم"**  >  **إلغاء تثبيت برنامج**.</span><span class="sxs-lookup"><span data-stu-id="1b97b-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="1b97b-119">أزاله [التثبيت باستخدام مساعد الإصلاح والدعم من Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت تعمل علي مشاكل.</span><span class="sxs-lookup"><span data-stu-id="1b97b-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.    <span data-ttu-id="1b97b-120">في RDS server ، سجل دخولك إلى مركز أداره Microsoft 365 باستخدام حساب المسؤول الخاص بك وقم [بتثبيت تطبيقات Microsoft 365 ل enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="1b97b-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.    <span data-ttu-id="1b97b-121">بعد تثبيت Office ، ***لا تقم بفتح اي من تطبيقات Office أو تسجيل الدخول*** اليه.</span><span class="sxs-lookup"><span data-stu-id="1b97b-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.    <span data-ttu-id="1b97b-122">في RDS server ، قم بتمكين تنشيط الكمبيوتر المشترك عن طريق تحرير السجل باتباع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="1b97b-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="1b97b-123">انقر بزر الماوس الأيمن فوق الشكل الموجود في الزاوية السفلية اليمني من الشاشة وحدد **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="1b97b-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="1b97b-124">في المربع فتح ، اكتب **regedit**، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="1b97b-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="1b97b-125">حدد **نعم** عندما تتم مطالبتك بالسماح لمحرر التسجيل باجراء تغييرات علي جهازك.</span><span class="sxs-lookup"><span data-stu-id="1b97b-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="1b97b-126">في "محرر السجل" ، أضف قيمه سلسله **شاريدكومبوتيرليسينسينج** باعداد 1 تحت HKEY_LOCAL_MACHINE \software\microsoft \office\clicktorun\configuration.</span><span class="sxs-lookup"><span data-stu-id="1b97b-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="1b97b-127">في RDS server ، ***سجل دخولك كمستخدم نهائي*** [وتحقق من تمكين تنشيط الكمبيوتر المشترك لتطبيقات Microsoft 365 ل enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="1b97b-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

