---
title: نشر الوظائف الإضافية Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233500"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="29190-102">نشر الوظائف الإضافية Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="29190-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="29190-103">النشر المركزي هو الطريقة المستحسنة لنشر Office الإضافية للمستخدمين والمجموعات داخل مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="29190-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="29190-104">لنشر الوظائف الإضافية، اتبع الخطوات أدناه:</span><span class="sxs-lookup"><span data-stu-id="29190-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="29190-105">**ملاحظة:** لتثبيت الوظائف الإضافية Office كمستخدم فردي، راجع عرض الوظائف الإضافية وإدارتها وتثبيتها في برامج [Office.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="29190-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="29190-106">تأكد أيضا من تمكين الحصول الفردي Office الإضافية 'لمتجر'.</span><span class="sxs-lookup"><span data-stu-id="29190-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="29190-107">للحصول على التفاصيل، راجع منع تنزيلات الوظائف الإضافية عن طريق إيقاف تشغيل Office عبر جميع العملاء [(باستثناء Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)</span><span class="sxs-lookup"><span data-stu-id="29190-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="29190-108">تأكد من أن بيئتك تلبي متطلبات نشر الوظائف الإضافية باستخدام النشر المركزي.</span><span class="sxs-lookup"><span data-stu-id="29190-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="29190-109">للحصول على التفاصيل، راجع [المتطلبات](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="29190-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="29190-110">انتقل إلى **الإعدادات** المتكاملة الحصول على التطبيقات في Microsoft 365 مركز الإدارة لنشر  >    >   الوظائف الإضافية.</span><span class="sxs-lookup"><span data-stu-id="29190-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="29190-111">ملاحظات:</span><span class="sxs-lookup"><span data-stu-id="29190-111">Notes:</span></span> 

- <span data-ttu-id="29190-112">تتطلب التطبيقات المتكاملة أن يكون المسؤول لديه أذونات المسؤول Exchange العام.</span><span class="sxs-lookup"><span data-stu-id="29190-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="29190-113">عند نشر الوظائف الإضافية لمستخدمين متعددين، نوصي بإجراء التعيينات باستخدام المجموعات بدلا من المستخدمين الفرديين.</span><span class="sxs-lookup"><span data-stu-id="29190-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="29190-114">للحصول على التفاصيل، راجع [الاعتبارات عند تعيين](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)مهمة إضافية للمستخدمين والمجموعات .</span><span class="sxs-lookup"><span data-stu-id="29190-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="29190-115">النشر المركزي لا يدعم المستخدمين في المجموعات المتداخلة أو المجموعات التي لديها مجموعات أصل.</span><span class="sxs-lookup"><span data-stu-id="29190-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="29190-116">للحصول على التفاصيل، راجع [تعيينات المستخدم والمجموعة](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span><span class="sxs-lookup"><span data-stu-id="29190-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="29190-117">تأكد من تمكين خدمة إدارة تطبيقات Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') للمستخدمين من تسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="29190-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="29190-118">للحصول على التفاصيل، راجع [تكوين خصائص التطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="29190-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="29190-119">إذا واجهت مشاكل في نشر الوظائف الإضافية باستخدام التطبيقات المتكاملة، فحاول النشر باستخدام [الوظائف الإضافية.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="29190-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="29190-120">لمزيد من المعلومات، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="29190-120">For more information, see:</span></span>

<span data-ttu-id="29190-121">[نشر الوظائف الإضافية في مركز الإدارة](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [إدارة الوظائف الإضافية في مركز الإدارة](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [استخدام Cmdlets للنشر المركزي في PowerShell لإدارة الوظائف الإضافية](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [نشر Office الإضافية باستخدام "النشر](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) المركزي" عبر Microsoft 365 مركز الإدارة 
 [استكشاف الأخطاء وإصلاحها: لا](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) يرى المستخدم الوظائف الإضافية 
 [استكشاف أخطاء المستخدم](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting) وإصلاحها باستخدام Office الإضافية</span><span class="sxs-lookup"><span data-stu-id="29190-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>