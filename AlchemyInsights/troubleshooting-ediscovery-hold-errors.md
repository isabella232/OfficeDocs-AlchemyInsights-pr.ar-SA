---
title: استكشاف أخطاء ediscovery وإصلاحها
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676021"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="b4242-102">استكشاف أخطاء ediscovery وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="b4242-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="b4242-103">هل تواجه مشاكل في عملية حفظ eDiscovery؟</span><span class="sxs-lookup"><span data-stu-id="b4242-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="b4242-104">فيما يلي بعض أفضل الممارسات التي يجب التفكير فيها:</span><span class="sxs-lookup"><span data-stu-id="b4242-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="b4242-105">تحقق من حالة توزيع الانتظار.</span><span class="sxs-lookup"><span data-stu-id="b4242-105">Check the hold distribution status.</span></span>  <span data-ttu-id="b4242-106">إذا كانت الحالة **قيد التشغيل (معلق)** أو إيقاف **التشغيل (معلق)،** فانتظر حتى اكتمال التوزيع الموضعي.</span><span class="sxs-lookup"><span data-stu-id="b4242-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="b4242-107">دمج التحديثات باستمرار في eDiscovery في طلب مجمع واحد بدلا من تحديث النهج بشكل متكرر لكل معاملة.</span><span class="sxs-lookup"><span data-stu-id="b4242-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="b4242-108">تشغيل Set-CaseHoldPolicy <policyname> -RetryDistribution في مركز الأمان والتوافق Powershell.</span><span class="sxs-lookup"><span data-stu-id="b4242-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="b4242-109">للحصول على التفاصيل، راجع الاتصال إلى & مركز التوافق [PowerShell](/powershell/exchange/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="b4242-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="b4242-110">للحصول على خطوات للتحقق من هذه الإعدادات وأفضل الممارسات الإضافية لتخفيف المشاكل التي تواجه eDiscovery وحلها، راجع استكشاف أخطاء الاحتفاظ ب [eDiscovery وإصلاحها](/microsoft-365/compliance/hold-distribution-errors).</span><span class="sxs-lookup"><span data-stu-id="b4242-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="b4242-111">للحصول على معلومات حول استكشاف مشاكل eDiscovery الشائعة الأخرى وإصلاحها، راجع التحقق من مشاكل [eDiscovery الشائعة وإصلاحها وحلها.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="b4242-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
