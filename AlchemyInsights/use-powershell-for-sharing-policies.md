---
title: استخدام PowerShell في نُهج المشاركة وعلاقات المؤسسة
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 9c52b876160f9577e6cefe7644c29d6fdf3b23fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826042"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="4347c-102">استخدام PowerShell في نُهج المشاركة وعلاقات المؤسسة</span><span class="sxs-lookup"><span data-stu-id="4347c-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="4347c-103">بالنسبة لعلاقات المؤسسة، رجاءً راجع بناء الجملة التفصيلي ومعلومات المعلمات لما يلي: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation)، و[New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship)، و[Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)، و[Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="4347c-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="4347c-104">لإنشاء نهج مشاركة، استخدم [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="4347c-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="4347c-105">[لتطبيق نهج مشاركة على صندوق بريد أو مستخدم](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)، يلزم استخدام مجموعة تتألف من  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) و[Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) مع النهج المُنشأ حديثاً.</span><span class="sxs-lookup"><span data-stu-id="4347c-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="4347c-106">[لتعديل نهج المشاركة أو تعطيله أو إزالته](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)، يلزم استخدام  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) و[Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="4347c-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="4347c-107">**للتوصل إلى فهم كامل لهذا الموضوع، رجاءً اقرأ:**</span><span class="sxs-lookup"><span data-stu-id="4347c-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="4347c-108">المشاركة في Exchange Online</span><span class="sxs-lookup"><span data-stu-id="4347c-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)