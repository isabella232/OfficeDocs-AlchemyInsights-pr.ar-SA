---
title: مشاكل الترخيص في Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657263"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="6a3e6-102">مشاكل الترخيص في Yammer</span><span class="sxs-lookup"><span data-stu-id="6a3e6-102">Yammer licensing issues</span></span>

<span data-ttu-id="6a3e6-103">يجب ان يتوفر لدي جميع المستخدمين ترخيص لاستخدام خدمه Yammer Enterprise ، ولكن لا يتطلب Yammer الافتراضي ان يملك المستخدمون ترخيصا للوصول إلى الخدمة.</span><span class="sxs-lookup"><span data-stu-id="6a3e6-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="6a3e6-104">عندما يقوم مسؤول بتغيير الاعداد لحظر مستخدمي Microsoft 365 بدون تراخيص Yammer ، لن يتمكن المستخدمون من تعيين ترخيص Yammer Enterprise علي خدمه Yammer.</span><span class="sxs-lookup"><span data-stu-id="6a3e6-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="6a3e6-105">لمزيد من المعلومات ، راجع [أداره تراخيص مستخدم Yammer في Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="6a3e6-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="6a3e6-106">عند أزاله التراخيص من المستخدمين ، لم تعد لوحه Yammer معروضه ، ويمكن للخدمات الأخرى استخدام أزاله الترخيص لإخفاء الميزات.</span><span class="sxs-lookup"><span data-stu-id="6a3e6-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="6a3e6-107">في بعض الحالات الأخرى ، لا يزال بإمكان الميزات ان تظهر ولكنه يتطلب تعيين ترخيص للعمل.</span><span class="sxs-lookup"><span data-stu-id="6a3e6-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="6a3e6-108">**لم يتم تحديث الترخيص للمستخدم**</span><span class="sxs-lookup"><span data-stu-id="6a3e6-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="6a3e6-109">في بعض الأحيان ، يتم تعيين ترخيص للمستخدم ولكن لا يزال يتعذر عليك الوصول إلى Yammer.</span><span class="sxs-lookup"><span data-stu-id="6a3e6-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="6a3e6-110">من المحتمل ان تحدث التاخيرات في حاله تقدم تعيين ترخيص كبير.</span><span class="sxs-lookup"><span data-stu-id="6a3e6-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="6a3e6-111">قد لا يتم تحديث مستخدمي Yammer بنفس الترتيب حيث يتم تغيير التراخيص في Azure AD لان النظام يعمل بشكل غير متزامن.</span><span class="sxs-lookup"><span data-stu-id="6a3e6-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="6a3e6-112">يمكنك الانتظار لمده 24 ساعة قبل فتح حاله دعم للإبلاغ عن مشاكل مزامنة الترخيص.</span><span class="sxs-lookup"><span data-stu-id="6a3e6-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="6a3e6-113">**تعيين ترخيص مجمع**</span><span class="sxs-lookup"><span data-stu-id="6a3e6-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="6a3e6-114">يمكن تعيين التراخيص من خلال مركز الاداره أو البرمجة النصية ل PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6a3e6-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="6a3e6-115">لمزيد من المعلومات ، راجع [تعيين تراخيص للمستخدمين](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) [وتعيين تراخيص لحسابات المستخدمين باستخدام Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="6a3e6-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="6a3e6-116">لا يوفر دعم Microsoft المساعدة في إنشاء البرامج النصية ، ولكن تتوفر الوثائق الموجودة علي تعيين ترخيص Yammer.</span><span class="sxs-lookup"><span data-stu-id="6a3e6-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="6a3e6-117">لمزيد من المعلومات ، راجع [أداره تراخيص Yammer باستخدام Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="6a3e6-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>