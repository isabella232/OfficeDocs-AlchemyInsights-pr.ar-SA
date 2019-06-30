---
title: 929 قواعد علبة الوارد إلى قواعد ديفليكترانسبورت
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/15/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6cf996e6d0a2698a5ce2bb57251de7c61d248d2a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35382652"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="16ca4-102">قواعد تدفق البريد (تعرف أيضا باسم قواعد النقل)</span><span class="sxs-lookup"><span data-stu-id="16ca4-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="16ca4-103">نظرة عامة حول قواعد تدفق البريد: [تدفق البريد القواعد (قواعد النقل) في Exchange عبر إنترنت](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="16ca4-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="16ca4-104">إعداد قواعد تدفق البريد: [تدفق البريد إجراءات القاعدة في Exchange عبر إنترنت](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="16ca4-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="16ca4-105">إنشاء وتعديل وحذف القواعد تدفق البريد: [إدارة قواعد تدفق البريد](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="16ca4-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="16ca4-106">يمكنك أيضا إدارة قواعد تدفق البريد في Exchange PowerShell عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="16ca4-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="16ca4-107">لمزيد من المعلومات، راجع [الحصول على ترانسبورترولي](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (عرض)، [ترانسبورترولي جديد](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (إنشاء)، [إزالة ترانسبورترولي](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (حذف)، و [مجموعة ترانسبورترولي](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (تعديل القائمة)، [ترانسبورترولي تعطيل](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (تعطيل القائمة)، و [تمكين ترانسبورترولي](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (تمكين القائمة).</span><span class="sxs-lookup"><span data-stu-id="16ca4-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="16ca4-108">Cmdlets القاعدة تدفق بريد إضافية: [الحصول على ترانسبورتروليكشن](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (قائمة الإجراءات المتاحة) و [الحصول على ترانسبورتروليبريديكاتي](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (قائمة الشروط المتاحة والاستثناءات)، [ترانسبورتروليكولكشن التصدير](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (قواعد التصدير) و [ استيراد ترانسبورتروليكولكشن](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (استيراد القواعد).</span><span class="sxs-lookup"><span data-stu-id="16ca4-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
