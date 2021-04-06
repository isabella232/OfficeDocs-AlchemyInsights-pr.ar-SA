---
title: أداة تشخيص الخدمة لسطح المكتب الظاهري ل Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595425"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="74705-102">أداة تشخيص الخدمة لسطح المكتب الظاهري ل Windows</span><span class="sxs-lookup"><span data-stu-id="74705-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="74705-103">يوفر Windows Virtual Desktop (WVD) أداة تشخيص تسمح للمسؤولين بتحديد الأخطاء من خلال واجهة واحدة.</span><span class="sxs-lookup"><span data-stu-id="74705-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="74705-104">تقوم هذه الأداة بتسجيل المعلومات ذات الصلة بالت تشخيص كلما تم استخدام WVD من قبل شخص تم تعيين دور WVD له.</span><span class="sxs-lookup"><span data-stu-id="74705-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="74705-105">يحتوي كل سجل على معلومات حول دور WVD الذي يتضمنه النشاط، ورسائل الخطأ التي تظهر أثناء جلسة العمل، ومعلومات حول المستأجر والمستخدم.</span><span class="sxs-lookup"><span data-stu-id="74705-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="74705-106">يمكن تكوين Azure Log Analytics لتسجيل سجل النشاط الذي أنشأته أداة التشخيص باتباع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="74705-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="74705-107">إنشاء مساحة عمل Log Analytics باستخدام [مدخل Azure](https://go.microsoft.com/fwlink/?linkid=2129500) أو [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="74705-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="74705-108">[توصيل أجهزة كمبيوتر Windows ب Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="74705-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="74705-109">احصل على "مفتاح مساحة العمل" والمفتاح الأساسي لمساحة العمل.</span><span class="sxs-lookup"><span data-stu-id="74705-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="74705-110">يحتاج معالج الإعداد إلى هذه المعلومات لتكوين الوكيل بشكل صحيح وضمان أنه يمكنه التواصل مع Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="74705-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="74705-111">[دفع البيانات التشخيصية إلى مساحة العمل.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="74705-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="74705-112">يمكنك نقل بيانات التشخيص من مستأجر WVD إلى Log Analytics لمساحة العمل.</span><span class="sxs-lookup"><span data-stu-id="74705-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="74705-113">[تحديد المشاكل](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) الداخلية أو الخارجية المتعلقة ب WVD وتشخصها.</span><span class="sxs-lookup"><span data-stu-id="74705-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="74705-114">لمعرفة المزيد حول تكوين أداة تشخيص الخدمة ل WVD، راجع استخدام تحليلات السجل لم الميزة التشخيصية.</span><span class="sxs-lookup"><span data-stu-id="74705-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>