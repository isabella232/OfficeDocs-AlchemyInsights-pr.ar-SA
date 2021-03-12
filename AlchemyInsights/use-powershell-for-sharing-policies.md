---
title: استخدام PowerShell في نُهج المشاركة وعلاقات المؤسسة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709453"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>استخدام PowerShell في نُهج المشاركة وعلاقات المؤسسة


بالنسبة لعلاقات المؤسسة، رجاءً راجع بناء الجملة التفصيلي ومعلومات المعلمات لما يلي: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation)، و[New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship)، و[Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)، و[Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

لإنشاء نهج مشاركة، استخدم [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). [لتطبيق نهج مشاركة على صندوق بريد أو مستخدم](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)، يلزم استخدام مجموعة تتألف من  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) و[Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) مع النهج المُنشأ حديثاً. [لتعديل نهج المشاركة أو تعطيله أو إزالته](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)، يلزم استخدام  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) و[Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**للتوصل إلى فهم كامل لهذا الموضوع، رجاءً اقرأ:**

[المشاركة في Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)