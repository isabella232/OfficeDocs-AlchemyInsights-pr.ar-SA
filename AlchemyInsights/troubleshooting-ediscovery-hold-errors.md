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
# <a name="troubleshooting-ediscovery-holds-errors"></a>استكشاف أخطاء ediscovery وإصلاحها

هل تواجه مشاكل في عملية حفظ eDiscovery؟ فيما يلي بعض أفضل الممارسات التي يجب التفكير فيها:

- تحقق من حالة توزيع الانتظار.  إذا كانت الحالة **قيد التشغيل (معلق)** أو إيقاف **التشغيل (معلق)،** فانتظر حتى اكتمال التوزيع الموضعي.
- دمج التحديثات باستمرار في eDiscovery في طلب مجمع واحد بدلا من تحديث النهج بشكل متكرر لكل معاملة.
- تشغيل Set-CaseHoldPolicy <policyname> -RetryDistribution في مركز الأمان والتوافق Powershell. للحصول على التفاصيل، راجع الاتصال إلى & مركز التوافق [PowerShell](/powershell/exchange/connect-to-scc-powershell).

للحصول على خطوات للتحقق من هذه الإعدادات وأفضل الممارسات الإضافية لتخفيف المشاكل التي تواجه eDiscovery وحلها، راجع استكشاف أخطاء الاحتفاظ ب [eDiscovery وإصلاحها](/microsoft-365/compliance/hold-distribution-errors).
للحصول على معلومات حول استكشاف مشاكل eDiscovery الشائعة الأخرى وإصلاحها، راجع التحقق من مشاكل [eDiscovery الشائعة وإصلاحها وحلها.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
