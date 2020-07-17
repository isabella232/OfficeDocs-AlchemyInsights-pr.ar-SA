---
title: استخدام PowerShell لنُهج المشاركة وعلاقات المؤسسة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862023"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="eaa69-102">استخدام PowerShell لنُهج المشاركة وعلاقات المؤسسة</span><span class="sxs-lookup"><span data-stu-id="eaa69-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="eaa69-103">لعلاقات المؤسسة الرجاء مراجعة بناء الجملة التفصيلية ومعلومات المعلمة لـ: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation)، [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship)، [تعيين- المنظمةRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) [وإزالة-المنظمة.](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship)</span><span class="sxs-lookup"><span data-stu-id="eaa69-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="eaa69-104">لإنشاء نهج المشاركة استخدم [سياسة المشاركة الجديدة](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="eaa69-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="eaa69-105">[لتطبيق نهج مشاركة على علبة بريد أو مستخدم](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) تحتاج إلى استخدام تركيبة من علبة البريد [مجموعة](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) [وعلبة الحصول مع](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) النهج الذي تم إنشاؤه حديثاً.</span><span class="sxs-lookup"><span data-stu-id="eaa69-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="eaa69-106">[لتعديل أو تعطيل أو إزالة نهج المشاركة](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) تحتاج إلى استخدام ["سياسة مشاركة Set-Sharing"](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) و ["إزالة-المشاركة السياسة](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="eaa69-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="eaa69-107">**لفهم هذا الموضوع بشكل كامل يرجى قراءة:**</span><span class="sxs-lookup"><span data-stu-id="eaa69-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="eaa69-108">المشاركة في Exchange عبر الإنترنت</span><span class="sxs-lookup"><span data-stu-id="eaa69-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)