---
title: تثبيت office علي خادم محطه طرفيه-غير مرخص
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663104"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="b3ba6-102">تثبيت Office علي خادم محطه طرفيه</span><span class="sxs-lookup"><span data-stu-id="b3ba6-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="b3ba6-103">بالنسبة إلى نشر تطبيقات Microsoft 365 للمؤسسة علي Windows Server باستخدام خدمات سطح المكتب البعيد (RDS) ، المسمية السابق الخدمات الطرفية:</span><span class="sxs-lookup"><span data-stu-id="b3ba6-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="b3ba6-104">يجب ان يتوفر لديك اشتراك Microsoft 365 يتضمن تطبيقات Microsoft 365 ل enterprise ، مثل Office 365 Enterprise E3 أو Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="b3ba6-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="b3ba6-105">لا تشمل تطبيقات Microsoft 365 للاعمال وتطبيقات Microsoft 365 لخطط business Premium تطبيقات Microsoft 365 ل enterprise.</span><span class="sxs-lookup"><span data-stu-id="b3ba6-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="b3ba6-106">أنت بحاجه إلى تمكين [تنشيط الكمبيوتر المشترك](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="b3ba6-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="b3ba6-107">إذا كنت تريد تثبيت تطبيقات Microsoft 365 ل enterprise علي RDS من Microsoft 365 admin center ، ***الذي يستخدم إعدادات التثبيت الافتراضية***، فاستخدم الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="b3ba6-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="b3ba6-108">يمكنك أيضا تنزيل [مساعد الإصلاح والدعم من microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) وتشغيله لتثبيت تطبيقات microsoft 365 ل enterprise في وضع تنشيط الكمبيوتر المشترك.</span><span class="sxs-lookup"><span data-stu-id="b3ba6-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="b3ba6-109">تحقق من اشتراك Microsoft 365 لديك.</span><span class="sxs-lookup"><span data-stu-id="b3ba6-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="b3ba6-110">تعرف علي كيفيه</span><span class="sxs-lookup"><span data-stu-id="b3ba6-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="b3ba6-111">إذا لزم الأمر ، فقم بالتبديل إلى اشتراك آخر في Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b3ba6-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="b3ba6-112">تعرف علي كيفيه</span><span class="sxs-lookup"><span data-stu-id="b3ba6-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="b3ba6-113">إذا كان Office مثبتا بالفعل علي خادم RDS باستخدام اي اشتراكات Microsoft 365 أخرى ، فقم بازاله تثبيته.</span><span class="sxs-lookup"><span data-stu-id="b3ba6-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="b3ba6-114">علي سبيل المثال ، بالانتقال إلى "لوحه التحكم" \> إلغاء تثبيت برنامج.</span><span class="sxs-lookup"><span data-stu-id="b3ba6-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="b3ba6-115">أزاله [التثبيت باستخدام مساعد الإصلاح والدعم من Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت تعمل علي مشاكل.</span><span class="sxs-lookup"><span data-stu-id="b3ba6-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="b3ba6-116">في RDS server ، سجل دخولك إلى مركز أداره Microsoft 365 باستخدام حساب المسؤول الخاص بك وقم [بتثبيت تطبيقات Microsoft 365 ل enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="b3ba6-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="b3ba6-117">بعد تثبيت Office ، ***لا تقم بفتح اي من تطبيقات Office أو تسجيل الدخول*** اليه.</span><span class="sxs-lookup"><span data-stu-id="b3ba6-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="b3ba6-118">في RDS server ، قم بتمكين تنشيط الكمبيوتر المشترك عن طريق تحرير السجل باتباع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="b3ba6-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="b3ba6-119">انقر بزر الماوس الأيمن في الزاوية السفلية اليمني من الشاشة وحدد تشغيل.</span><span class="sxs-lookup"><span data-stu-id="b3ba6-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="b3ba6-120">في المربع فتح ، اكتب **regedit**، ثم حدد موافق.</span><span class="sxs-lookup"><span data-stu-id="b3ba6-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="b3ba6-121">حدد نعم عندما تتم مطالبتك بالسماح لمحرر التسجيل باجراء تغييرات علي جهازك.</span><span class="sxs-lookup"><span data-stu-id="b3ba6-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="b3ba6-122">في "محرر السجل" ، أضف قيمه سلسله **شاريدكومبوتيرليسينسينج** باعداد 1 تحت HKEY_LOCAL_MACHINE \software\microsoft \office\clicktorun\configuration.</span><span class="sxs-lookup"><span data-stu-id="b3ba6-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="b3ba6-123">في RDS server ، ***سجل دخولك كمستخدم نهائي*** [وتحقق من تمكين تنشيط الكمبيوتر المشترك لتطبيقات Microsoft 365 ل enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="b3ba6-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="b3ba6-124">للحصول علي مزيد من التفاصيل حول المتطلبات الاساسيه ، قم باعداد الإرشادات والإرشادات علي التثبيتات المخصصة باستخدام أداه نشر Office ، الرجاء مراجعه [نشر تطبيقات Microsoft 365 للمؤسسة باستخدام خدمات سطح المكتب البعيد](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="b3ba6-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="b3ba6-125">لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشترك ، يرجى مراجعه [استكشاف الأخطاء وإصلاحها في تنشيط الكمبيوتر المشترك لتطبيقات Microsoft 365 ل enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="b3ba6-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  