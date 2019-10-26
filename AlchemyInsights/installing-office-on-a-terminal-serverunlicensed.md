---
title: تثبيت office علي ملقم المحطة الطرفية-غير مرخص
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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/25/2019
ms.locfileid: "37205396"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="ede4e-102">تثبيت Office علي ملقم المحطة الطرفية</span><span class="sxs-lookup"><span data-stu-id="ede4e-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="ede4e-103">لنشر Office 365 ProPlus علي ملقم Windows باستخدام خدمات سطح المكتب البعيد (RDS) ، المسمية سابقا "الخدمات الطرفية":</span><span class="sxs-lookup"><span data-stu-id="ede4e-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="ede4e-104">يجب ان يكون لديك خطه 365 Office التي تتضمن Office 365 ProPlus ، مثل Office 365 المؤسسة E3 أو المؤسسة E5.</span><span class="sxs-lookup"><span data-stu-id="ede4e-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="ede4e-105">لا تتضمن خطط office 365 الاعمال والمكتب 365 Premium الاعمال Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="ede4e-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="ede4e-106">تحتاج إلى تمكين [تنشيط الكمبيوتر المشترك](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="ede4e-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="ede4e-107">إذا كنت ترغب في تثبيت Office 365 ProPlus علي RDS من مركز مسؤول Microsoft 365 ، ***الذي يستخدم إعدادات التثبيت الافتراضية***، اتبع الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="ede4e-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="ede4e-108">يمكنك أيضا تحميل وتشغيل [مساعد الدعم والاسترداد ل Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) لتثبيت Office 365 proplus في وضع تنشيط الكمبيوتر المشترك.</span><span class="sxs-lookup"><span data-stu-id="ede4e-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="ede4e-109">تحقق من خطه Office 365 التي لديك.</span><span class="sxs-lookup"><span data-stu-id="ede4e-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="ede4e-110">تعرف علي كيفيه</span><span class="sxs-lookup"><span data-stu-id="ede4e-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="ede4e-111">إذا لزم الأمر ، قم بالتبديل إلى خطه 365 Office مختلفه.</span><span class="sxs-lookup"><span data-stu-id="ede4e-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="ede4e-112">تعرف علي كيفيه</span><span class="sxs-lookup"><span data-stu-id="ede4e-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="ede4e-113">إذا كان Office مثبتا بالفعل علي ملقم RDS باستخدام إيه خطط Office 365 أخرى ، إلغاء تثبيته.</span><span class="sxs-lookup"><span data-stu-id="ede4e-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="ede4e-114">علي سبيل المثال ، عن طريق الانتقال إلى "لوحه التحكم" \> إلغاء تثبيت برنامج.</span><span class="sxs-lookup"><span data-stu-id="ede4e-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="ede4e-115">إلغاء [التثبيت باستخدام دعم Microsoft ومساعد الاسترداد](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت قيد التشغيل في المشكلات.</span><span class="sxs-lookup"><span data-stu-id="ede4e-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="ede4e-116">علي ملقم RDS تسجيل الدخول إلى مركز مسؤول Microsoft 365 مع حساب المسؤول [وتثبيت Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="ede4e-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="ede4e-117">بعد تثبيت Office ، ***لا تقم بفتح أو تسجيل*** الدخول إلى اي من تطبيقات office.</span><span class="sxs-lookup"><span data-stu-id="ede4e-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="ede4e-118">علي ملقم RDS تمكين تنشيط الكمبيوتر المشتركة عن طريق تحرير التسجيل باتباع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="ede4e-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="ede4e-119">انقر نقرا ايمن فوق زر Windows في الزاوية السفلية اليمني من الشاشة وحدد تشغيل.</span><span class="sxs-lookup"><span data-stu-id="ede4e-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="ede4e-120">في المربع فتح ، اكتب **regedit**، ثم حدد موافق.</span><span class="sxs-lookup"><span data-stu-id="ede4e-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="ede4e-121">حدد نعم عند مطالبتك بالسماح لمحرر التسجيل باجراء تغييرات علي جهازك.</span><span class="sxs-lookup"><span data-stu-id="ede4e-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="ede4e-122">في "محرر التسجيل" ، أضافه قيمه سلسله من **Sharedالكمبيوادالترخيص** مع اعداد من 1 ضمن HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Date\clortorun\contate.</span><span class="sxs-lookup"><span data-stu-id="ede4e-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="ede4e-123">علي ملقم RDS ***تسجيل الدخول كمستخدم نهائي*** [وتحقق من تمكين تنشيط الكمبيوتر المشتركة ل Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="ede4e-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="ede4e-124">لمزيد من التفاصيل حول المتطلبات الاساسيه ، إرشادات الاعداد وإرشادات حول عمليات التثبيت المخصصة باستخدام أداه نشر Office ، الرجاء مراجعه [نشر office 365 ProPlus باستخدام "خدمات سطح المكتب البعيد](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)".</span><span class="sxs-lookup"><span data-stu-id="ede4e-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="ede4e-125">لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشتركة ، الرجاء مراجعه [استكشاف المشكلات وإصلاحها مع تنشيط الكمبيوتر المشترك ل Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="ede4e-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  