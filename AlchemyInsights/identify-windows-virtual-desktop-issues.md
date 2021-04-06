---
title: تحديد مشاكل سطح المكتب الظاهري ل Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595424"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="6130e-102">تحديد مشاكل سطح المكتب الظاهري ل Windows</span><span class="sxs-lookup"><span data-stu-id="6130e-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="6130e-103">يستخدم Windows Virtual Desktop Diagnostics أمر cmdlet واحد فقط من PowerShell ولكنه يحتوي على العديد من المعلمات الاختيارية للمساعدة في تضييق المشاكل وعزلها.</span><span class="sxs-lookup"><span data-stu-id="6130e-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="6130e-104">للبدء:</span><span class="sxs-lookup"><span data-stu-id="6130e-104">To get started:</span></span> 

1. <span data-ttu-id="6130e-105">قم بتنزيل الوحدة النمطية لسطح المكتب الظاهري ل Windows PowerShell واستيرادها.</span><span class="sxs-lookup"><span data-stu-id="6130e-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="6130e-106">للحصول على التفاصيل، راجع [Windows Virtual Desktop Cmdlets ل Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span><span class="sxs-lookup"><span data-stu-id="6130e-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="6130e-107">قم بتشغيل cmdlet التالي تسجيل الدخول إلى حسابك:</span><span class="sxs-lookup"><span data-stu-id="6130e-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="6130e-108">مثال: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="6130e-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="6130e-109">**ملاحظة:** يجب أن تتضمن كل الاستعلامات التي تستخدم PowerShell المعلمتين -UserName أو -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="6130e-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="6130e-110">للحصول على قدرات المراقبة، راجع [استخدام Log Analytics لمميزة التشخيص](https://go.microsoft.com/fwlink/?linkid=2126847).</span><span class="sxs-lookup"><span data-stu-id="6130e-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="6130e-111">لتصفية الأنشطة التشخيصية حسب المستخدم، يمكنك تشغيل cmdlet التالي:</span><span class="sxs-lookup"><span data-stu-id="6130e-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="6130e-112">مثال: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="6130e-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="6130e-113">توجد قائمة عوامل التصفية التي يمكنك تشغيلها لتشخيص المشاكل.</span><span class="sxs-lookup"><span data-stu-id="6130e-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="6130e-114">لمعرفة المزيد حول تشخيص المشاكل، راجع التعرف على مشاكل سطح المكتب الظاهري ل [Windows وتشخصها](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="6130e-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="6130e-115">لمعرفة المزيد حول الأخطاء الشائعة، راجع الأخطاء الشائعة [senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="6130e-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
