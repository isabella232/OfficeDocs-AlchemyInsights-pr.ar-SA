---
title: مشكلات ترخيص Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148166"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="80650-102">مشكلات ترخيص Yammer</span><span class="sxs-lookup"><span data-stu-id="80650-102">Yammer licensing issues</span></span>

<span data-ttu-id="80650-103">يجب أن يكون لدى كافة المستخدمين ترخيص لاستخدام خدمة "المؤسسة Yammer" ولكن افتراضياً لا يتطلب Yammer أن يكون لدى المستخدمين ترخيص الوصول إلى الخدمة.</span><span class="sxs-lookup"><span data-stu-id="80650-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="80650-104">عندما يقوم مسؤول بتغيير الإعداد لحظر مستخدمي Microsoft 365 بدون تراخيص Yammer، لا يمكن للمستخدمين الذين لم يتم تعيين ترخيص شركة Yammer الوصول إلى خدمة Yammer.</span><span class="sxs-lookup"><span data-stu-id="80650-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="80650-105">لمزيد من المعلومات، راجع [إدارة تراخيص المستخدمين Yammer في Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="80650-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="80650-106">عند إزالة التراخيص من المستخدمين، لم يعد يتم عرض الإطار المتجانب Yammer، كما يمكن استخدام خدمات أخرى إزالة الترخيص لإخفاء الميزات.</span><span class="sxs-lookup"><span data-stu-id="80650-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="80650-107">وفي حالات أخرى، يمكن أن تظل الميزات تظهر ولكنها تتطلب تخصيص ترخيص للعمل.</span><span class="sxs-lookup"><span data-stu-id="80650-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="80650-108">**الترخيص لا يتم تحديث للمستخدم**</span><span class="sxs-lookup"><span data-stu-id="80650-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="80650-109">أحياناً، يتم تعيين ترخيص مستخدم ولكن لا يزال غير قادر على الوصول Yammer.</span><span class="sxs-lookup"><span data-stu-id="80650-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="80650-110">من المحتمل حدوث التأخيرات عند وجود مهمة ترخيص كبيرة قيد التقدم.</span><span class="sxs-lookup"><span data-stu-id="80650-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="80650-111">قد لا يتم تحديث المستخدمين Yammer بنفس الترتيب كما يتم تغيير التراخيص في إعلان Azure لأن النظام يعمل بشكل غير متزامن.</span><span class="sxs-lookup"><span data-stu-id="80650-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="80650-112">انتظر حتى 24 ساعة قبل فتح حالة دعم للإبلاغ عن مشكلات مزامنة الترخيص.</span><span class="sxs-lookup"><span data-stu-id="80650-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="80650-113">**تعيين الترخيص المجمع**</span><span class="sxs-lookup"><span data-stu-id="80650-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="80650-114">يمكن تعيين التراخيص من خلال مركز الإدارة أو برمجة PowerShell النصية.</span><span class="sxs-lookup"><span data-stu-id="80650-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="80650-115">لمزيد من المعلومات، راجع [تعيين التراخيص للمستخدمين](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) [وتعيين التراخيص لحسابات المستخدمين باستخدام Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="80650-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="80650-116">لا يوفر دعم Microsoft المساعدة في إنشاء البرامج النصية، ولكن تتوفر الوثائق الموجودة على تعيين ترخيص Yammer.</span><span class="sxs-lookup"><span data-stu-id="80650-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="80650-117">لمزيد من المعلومات، راجع [إدارة تراخيص Yammer باستخدام Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="80650-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>