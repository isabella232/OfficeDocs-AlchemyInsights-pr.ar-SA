---
title: تثبيت المكتب على خادم المحطة الطرفية - غير مرخص
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508615"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="33411-102">تثبيت Office على خادم المحطة الطرفية</span><span class="sxs-lookup"><span data-stu-id="33411-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="33411-103">لنشر تطبيقات Microsoft 365 للمؤسسات على خادم Windows باستخدام خدمات سطح المكتب البعيد (RDS)، التي كانت تسمى سابقًا خدمات المحطة الطرفية:</span><span class="sxs-lookup"><span data-stu-id="33411-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="33411-104">يجب أن يكون لديك اشتراك Microsoft 365 يتضمن تطبيقات Microsoft 365 للمؤسسات، مثل Office 365 Enterprise E3 أو Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="33411-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="33411-105">لا تتضمن تطبيقات Microsoft 365 للأعمال وتطبيقات Microsoft 365 لخطط Premium للأعمال تطبيقات Microsoft 365 للمؤسسات.</span><span class="sxs-lookup"><span data-stu-id="33411-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="33411-106">تحتاج إلى تمكين [تنشيط الكمبيوتر المشترك](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="33411-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="33411-107">إذا كنت ترغب في تثبيت تطبيقات Microsoft 365 للمؤسسات على RDS من مركز إدارة Microsoft 365، ***والذي يستخدم إعدادات التثبيت الافتراضية،*** فاستخدم الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="33411-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="33411-108">يمكنك أيضًا تنزيل [وتشغيل مساعد دعم واسترداد Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) لتثبيت تطبيقات Microsoft 365 للمؤسسات في وضع تنشيط الكمبيوتر المشترك.</span><span class="sxs-lookup"><span data-stu-id="33411-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="33411-109">تحقق من اشتراك Microsoft 365 لديك.</span><span class="sxs-lookup"><span data-stu-id="33411-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="33411-110">تعرف على كيفية</span><span class="sxs-lookup"><span data-stu-id="33411-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="33411-111">إذا لزم الأمر، قم بالتبديل إلى اشتراك Microsoft 365 مختلف.</span><span class="sxs-lookup"><span data-stu-id="33411-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="33411-112">تعرف على كيفية</span><span class="sxs-lookup"><span data-stu-id="33411-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="33411-113">إذا تم تثبيت Office بالفعل على خادم RDS باستخدام أي اشتراكات Microsoft 365 الأخرى، فقم بإلغاء تثبيته.</span><span class="sxs-lookup"><span data-stu-id="33411-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="33411-114">على سبيل المثال، عن طريق الانتقال إلى لوحة التحكم \> إلغاء تثبيت برنامج.</span><span class="sxs-lookup"><span data-stu-id="33411-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="33411-115">إلغاء التثبيت باستخدام [مساعد دعم Microsoft والاسترداد](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت تقوم بمشكلات.</span><span class="sxs-lookup"><span data-stu-id="33411-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="33411-116">على خادم RDS، قم بتسجيل الدخول إلى مركز إدارة Microsoft 365 باستخدام حساب المسؤول [وتثبيت تطبيقات Microsoft 365 للمؤسسات](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="33411-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="33411-117">بعد تثبيت Office، ***لا تفتح أو تسجل الدخول*** إلى أي تطبيقات Office.</span><span class="sxs-lookup"><span data-stu-id="33411-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="33411-118">على ملقم RDS، تمكين تنشيط الكمبيوتر المشترك عن طريق تحرير التسجيل باتباع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="33411-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="33411-119">انقر بزر Windows في الزاوية اليسرى السفلى من الشاشة وحدد تشغيل.</span><span class="sxs-lookup"><span data-stu-id="33411-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="33411-120">في المربع المفتوح، اكتب **regedit**، ثم حدد موافق.</span><span class="sxs-lookup"><span data-stu-id="33411-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="33411-121">حدد نعم عندما تتم مطالبتك بالسماح لمحرر التسجيل بإجراء تغييرات على جهازك.</span><span class="sxs-lookup"><span data-stu-id="33411-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="33411-122">في محرر التسجيل، قم بإضافة قيمة سلسلة من **SharedComputerLicensing** مع إعداد 1 تحت HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="33411-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="33411-123">على خادم RDS، ***قم بتسجيل الدخول كمستخدم نهائي*** وتحقق من تمكين تنشيط الكمبيوتر المشترك لتطبيقات Microsoft [365 للمؤسسات](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="33411-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="33411-124">لمزيد من التفاصيل حول المتطلبات الأساسية وإرشادات الإعداد والإرشادات حول المنشآت المخصصة باستخدام أداة نشر Office، يرجى الاطلاع [على نشر تطبيقات Microsoft 365 للمؤسسات باستخدام خدمات سطح المكتب البعيد](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="33411-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="33411-125">لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشترك، يرجى الاطلاع على [مشكلات استكشاف الأخطاء وإصلاحها المتعلقة بتنشيط الكمبيوتر المشترك لتطبيقات Microsoft 365 للمؤسسات](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="33411-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  