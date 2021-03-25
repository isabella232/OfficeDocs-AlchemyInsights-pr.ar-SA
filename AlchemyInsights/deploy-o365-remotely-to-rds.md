---
title: نشر تطبيقات Microsoft 365 للمؤسسات للاستخدام المشترك على RDS أو Terminal Server أو VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200660"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="63506-102">نشر تطبيقات Microsoft 365 للمؤسسات للاستخدام المشترك على RDS أو Terminal Server أو VDI</span><span class="sxs-lookup"><span data-stu-id="63506-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="63506-103">لنشر تطبيقات Microsoft 365 للمؤسسات باستخدام خدمات سطح المكتب البعيد (RDS)، التي كانت تسمى سابقا خدمات المحطة الطرفية:</span><span class="sxs-lookup"><span data-stu-id="63506-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="63506-104">يجب أن يكون لديك خطة Microsoft 365 for Business أو خطة Office 365 تتضمن تطبيقات Microsoft 365 للمؤسسات، مثل Office 365 Enterprise E3 أو Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="63506-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="63506-105">لا تتضمن خطط Microsoft 365 Apps للأعمال و Microsoft 365 Business Standard تطبيقات Microsoft 365 للمؤسسات.</span><span class="sxs-lookup"><span data-stu-id="63506-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="63506-106">يجب تمكين تنشيط [الكمبيوتر المشترك](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="63506-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="63506-107">يمكنك أيضا تنزيل مساعد الاسترداد والدعم [من Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) وتشغيله لتثبيت تطبيقات Microsoft 365 للمؤسسات في وضع تنشيط الكمبيوتر المشترك.</span><span class="sxs-lookup"><span data-stu-id="63506-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="63506-108">لمزيد من المعلومات حول المتطلبات الأساسية وإرشادات الإعداد والإرشادات حول عمليات التثبيت المخصصة باستخدام أداة نشر Office، راجع نشر [تطبيقات Microsoft 365](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)للمؤسسات باستخدام خدمات سطح المكتب البعيد .</span><span class="sxs-lookup"><span data-stu-id="63506-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="63506-109">لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشترك:</span><span class="sxs-lookup"><span data-stu-id="63506-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="63506-110">راجع استكشاف المشاكل المتعلقة بتنشيط الكمبيوتر المشترك وإصلاحها [لتطبيقات Microsoft 365 للمؤسسات](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="63506-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="63506-111">راجع [إعادة تعيين تطبيقات Microsoft 365 لحالة تفعيل المؤسسة](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="63506-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="63506-112">إذا كنت تريد تثبيت تطبيقات Microsoft 365 للمؤسسات على RDS من مركز إدارة Microsoft 365، الذي يستخدم إعدادات التثبيت الافتراضية، فاتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="63506-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="63506-113">تحقق من الاشتراك الذي تملكه.</span><span class="sxs-lookup"><span data-stu-id="63506-113">Check what subscription you have.</span></span> <span data-ttu-id="63506-114">[تعرف على كيفية](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="63506-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="63506-115">إذا لزم الأمر، قم بالتبديل إلى اشتراك آخر.</span><span class="sxs-lookup"><span data-stu-id="63506-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="63506-116">[تعرف على كيفية](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="63506-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="63506-117">إذا كان Office مثبتا بالفعل على خادم RDS باستخدام أي اشتراكات Microsoft أخرى، ف إلغاء تثبيته.</span><span class="sxs-lookup"><span data-stu-id="63506-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="63506-118">على سبيل المثال، عن طريق الذهاب إلى **لوحة التحكم** إلغاء  >  **تثبيت برنامج**.</span><span class="sxs-lookup"><span data-stu-id="63506-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="63506-119">إلغاء التثبيت باستخدام مساعد الاسترداد [والدعم من Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت تخوض مشاكل.</span><span class="sxs-lookup"><span data-stu-id="63506-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="63506-120">على خادم RDS، سجل الدخول إلى مركز إدارة Microsoft 365 باستخدام حساب المسؤول وثبت [تطبيقات Microsoft 365 للمؤسسات](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="63506-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="63506-121">بعد تثبيت ***Office، لا*** تفتح أو سجل الدخول إلى أي من تطبيقات Office.</span><span class="sxs-lookup"><span data-stu-id="63506-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="63506-122">على خادم RDS، قم بتمكين تنشيط الكمبيوتر المشترك عن طريق تحرير السجل باتباع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="63506-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="63506-123">انقر بزر الماوس الأيمن فوق زر Windows في الزاوية السفلية اليمنى من الشاشة وحدد **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="63506-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="63506-124">في المربع فتح، اكتب **regedit**، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="63506-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="63506-125">حدد **نعم** عند مطالبتك بالسماح لمحرر السجل بإجراء تغييرات على جهازك.</span><span class="sxs-lookup"><span data-stu-id="63506-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="63506-126">في محرر السجل، أضف قيمة سلسلة **ل SharedComputerLicensing** بإعداد 1 ضمن HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="63506-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="63506-127">على خادم RDS، سجل الدخول كمستخدم وتحقق من تمكين تنشيط الكمبيوتر المشترك  [لتطبيقات Microsoft 365 للمؤسسات.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)</span><span class="sxs-lookup"><span data-stu-id="63506-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>
