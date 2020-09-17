---
title: 929 قواعد علبه الوارد إلى قواعد ديفليكترانسبورت
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: abb729c40fb87bcca8cc03c95aa4677597d20c08
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778678"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="874c8-102">قواعد تدفق البريد (المعروفة أيضا باسم قواعد النقل)</span><span class="sxs-lookup"><span data-stu-id="874c8-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="874c8-103">نظره عامه عامه حول قواعد تدفق البريد: [قواعد تدفق البريد (قواعد النقل) في Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="874c8-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="874c8-104">اعداد قواعد تدفق البريد: [إجراءات قواعد تدفق البريد في Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="874c8-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="874c8-105">إنشاء قواعد تدفق البريد وتعديلها وحذفها: [أداره قواعد تدفق البريد](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="874c8-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="874c8-106">يمكنك أيضا أداره قواعد تدفق البريد في Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="874c8-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="874c8-107">للحصول علي مزيد من المعلومات ، راجع [ترانسبورترولي](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (عرض) ، [ترانسبورترولي](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (إنشاء) ، [أزاله-ترانسبورترولي](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (حذف) ، [تعيين-ترانسبورترولي](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (تعديل موجود) ، [وتمكين-ترانسبورترولي (تمكين الوصول](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) اليه) ، [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule)</span><span class="sxs-lookup"><span data-stu-id="874c8-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="874c8-108">أوامر cmdlets لقاعده البريد [الاضافيه: ترانسبورتروليكتيون (الإجراءات المتوفرة](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) ) ، والحصول علي [ترانسبورتروليبريديكاتي (الشروط](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) المتاحة والاستثناءات) ، [والتصدير-ترانسبورتروليكولكتيون](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (تصدير القواعد) ، [والاستيراد-ترانسبورتروليكولكتيون](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (استيراد القواعد).</span><span class="sxs-lookup"><span data-stu-id="874c8-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
