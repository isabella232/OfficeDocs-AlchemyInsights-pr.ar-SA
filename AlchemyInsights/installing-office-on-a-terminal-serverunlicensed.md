---
title: تثبيت المكتب على ملقم المحطة الطرفية - غير مرخص
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735376"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="803be-102">تثبيت Office على ملقم المحطة طرفية</span><span class="sxs-lookup"><span data-stu-id="803be-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="803be-103">لنشر Office 365 ProPlus على ملقم Windows باستخدام خدمات سطح المكتب البعيد (RDS)، التي كانت تسمى سابقاً "الخدمات الطرفية":</span><span class="sxs-lookup"><span data-stu-id="803be-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="803be-104">يجب أن يكون لديك خطة Office 365 التي تتضمن Office 365 ProPlus، مثل Office 365 المؤسسة E3 أو المؤسسة E5.</span><span class="sxs-lookup"><span data-stu-id="803be-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="803be-105">لا تتضمن خطط Office 365 الأعمال وOffice 365 الأعمال بريميوم Office 365.</span><span class="sxs-lookup"><span data-stu-id="803be-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="803be-106">تحتاج إلى تمكين [تنشيط الكمبيوتر المشترك](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="803be-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="803be-107">إذا كنت ترغب في تثبيت Office 365 ProPlus على RDS من مركز مسؤول Microsoft 365 ***الذي يستخدم إعدادات التثبيت الافتراضية***اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="803be-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="803be-108">تحقق من خطة Office 365 لديك.</span><span class="sxs-lookup"><span data-stu-id="803be-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="803be-109">تعرّف على كيفية</span><span class="sxs-lookup"><span data-stu-id="803be-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="803be-110">إذا لزم الأمر، قم بالتبديل إلى خطة Office 365 مختلفة.</span><span class="sxs-lookup"><span data-stu-id="803be-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="803be-111">تعرّف على كيفية</span><span class="sxs-lookup"><span data-stu-id="803be-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="803be-112">إذا كان Office مثبتًا بالفعل على ملقم RDS باستخدام أي خطط Office 365 أخرى، فقم بإلغاء تثبيته.</span><span class="sxs-lookup"><span data-stu-id="803be-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="803be-113">على سبيل المثال، عن \> طريق الانتقال إلى "لوحة التحكم" إلغاء تثبيت برنامج.</span><span class="sxs-lookup"><span data-stu-id="803be-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="803be-114">إلغاء التثبيت باستخدام [مساعد الدعم والاسترداد لـ Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت تعمل على مشكلات.</span><span class="sxs-lookup"><span data-stu-id="803be-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="803be-115">على ملقم RDS، قم بتسجيل الدخول إلى مركز مسؤول Microsoft 365 مع حساب المسؤول الخاص بك [وتثبيت Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="803be-115">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="803be-116">بعد تثبيت Office، لا تقم بفتح أي تطبيقات Office ***أو تسجيل الدخول*** إليها.</span><span class="sxs-lookup"><span data-stu-id="803be-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="803be-117">على ملقم RDS تمكين تنشيط الكمبيوتر المشترك عن طريق تحرير التسجيل باتباع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="803be-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="803be-118">انقر بزر الماوس الأيمن فوق زر Windows في الركن الأيمن السفلي من الشاشة وحدد تشغيل.</span><span class="sxs-lookup"><span data-stu-id="803be-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="803be-119">في المربع فتح ، اكتب **regedit**، ثم حدد موافق.</span><span class="sxs-lookup"><span data-stu-id="803be-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="803be-120">حدد نعم عند مطالبتك بالسماح لمحرر التسجيل بإجراء تغييرات على جهازك.</span><span class="sxs-lookup"><span data-stu-id="803be-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="803be-121">في "محرر التسجيل" إضافة قيمة سلسلة **SharedComputerLicensing** مع إعداد 1 ضمن HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="803be-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="803be-122">على ملقم RDS تسجيل ***الدخول كمستخدم نهائي*** [وتحقق من تمكين تنشيط الكمبيوتر المشترك ل Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="803be-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="803be-123">لمزيد من التفاصيل حول المتطلبات المسبقة وإرشادات الإعداد والإرشادات حول عمليات التثبيت المخصصة باستخدام أداة نشر Office، الرجاء [مراجعة نشر Office 365 ProPlus باستخدام "خدمات سطح المكتب البعيد".](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)</span><span class="sxs-lookup"><span data-stu-id="803be-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="803be-124">لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشترك، الرجاء [استكشاف مشكلات تنشيط الكمبيوتر المشترك لـ Office 365 ProPlus وإصلاحها.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="803be-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  