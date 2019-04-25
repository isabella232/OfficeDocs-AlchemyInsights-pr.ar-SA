---
title: تثبيت office على "ملقم المحطة الطرفية"-غير مرخص
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32410109"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="8053f-102">تثبيت Office على ملقم المحطة الطرفية</span><span class="sxs-lookup"><span data-stu-id="8053f-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="8053f-103">لنشر Office 365 ProPlus على خادم Windows استخدام خدمات سطح المكتب البعيد (RDS)، المعروف فيما مضى "الخدمات الطرفية":</span><span class="sxs-lookup"><span data-stu-id="8053f-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="8053f-104">يجب أن يكون لديك مخطط Office 365 يتضمن Office 365 ProPlus، مثل Office 365 المؤسسة E3 أو E5 المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="8053f-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="8053f-105">لا يتم تضمين خطط العمل 365 Office و Office 365 الأعمال الأولية Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="8053f-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="8053f-106">تحتاج إلى تمكين [تنشيط الكمبيوتر المشتركة](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="8053f-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="8053f-107">إذا أردت تثبيت Office 365 ProPlus على RDS من المدخل Office 365، \* \* *التي تستخدم إعدادات التثبيت الافتراضي* \* \*، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="8053f-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="8053f-108">تحقق من خطة Office 365 ما لديك.</span><span class="sxs-lookup"><span data-stu-id="8053f-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="8053f-109">التعرف على كيفية</span><span class="sxs-lookup"><span data-stu-id="8053f-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. <span data-ttu-id="8053f-110">إذا لزم الأمر، قم بالتبديل إلى Office 365 مختلفة تخطط.</span><span class="sxs-lookup"><span data-stu-id="8053f-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="8053f-111">التعرف على كيفية</span><span class="sxs-lookup"><span data-stu-id="8053f-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. <span data-ttu-id="8053f-112">إذا كان Office مثبتاً على RDS server استخدام أي خطط Office 365، إلغاء تثبيته.</span><span class="sxs-lookup"><span data-stu-id="8053f-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="8053f-113">على سبيل المثال، عن طريق الانتقال إلى "لوحة التحكم" \> بإلغاء تثبيت برنامج.</span><span class="sxs-lookup"><span data-stu-id="8053f-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="8053f-114">إلغاء استخدام [دعم Microsoft ومساعد الاسترداد](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت تشغل في القضايا.</span><span class="sxs-lookup"><span data-stu-id="8053f-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="8053f-115">على RDS server، تسجيل الدخول إلى موقع Office 365 باستخدام حساب المسؤول و [تثبيت Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="8053f-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="8053f-116">بعد تثبيت Office، \* \* *عدم فتح أو تسجيل الدخول* \* \* لأي من تطبيقات Office.</span><span class="sxs-lookup"><span data-stu-id="8053f-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="8053f-117">على RDS server تمكين تنشيط الكمبيوتر المشترك بتحرير التسجيل باتباع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="8053f-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="8053f-118">انقر فوق الزر Windows في الزاوية السفلي اليسرى من الشاشة، وحدد تشغيل.</span><span class="sxs-lookup"><span data-stu-id="8053f-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="8053f-119">في المربع فتح، اكتب **regedit**، ومن ثم حدد "موافق".</span><span class="sxs-lookup"><span data-stu-id="8053f-119">In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="8053f-120">حدد نعم عندما يطلب منك السماح "محرر التسجيل" لإجراء تغييرات على الجهاز الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="8053f-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="8053f-121">في "محرر التسجيل"، إضافة قيمة سلسلة من **شاريدكومبوتيرليسينسينج** بإعداد 1 تحت HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="8053f-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="8053f-122">على RDS server \* \* *تسجيل الدخول كمستخدم نهائي* \* \* و [تحقق من أنه تم تمكين تنشيط الكمبيوتر المشتركة ل Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="8053f-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="8053f-123">لمزيد من التفاصيل حول المتطلبات المسبقة والإرشادات والتوجيهات بشأن عمليات التثبيت المخصص باستخدام أداة نشر Office، الرجاء مراجعة [توزيع Office 365 ProPlus باستخدام "خدمات سطح المكتب البعيد"](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="8053f-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="8053f-124">لحل الأخطاء المتعلقة بتنشيط الكمبيوتر المشتركة، راجع [استكشاف مشكلات تنشيط الكمبيوتر المشتركة ل Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="8053f-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

