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
ms.openlocfilehash: 48df03b1397b0e924aa878cea3d1cac07ca862c3636c1273d10f4841a03fddcf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998453"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>استخدام PowerShell في نُهج المشاركة وعلاقات المؤسسة


بالنسبة لعلاقات المؤسسة، رجاءً راجع بناء الجملة التفصيلي ومعلومات المعلمات لما يلي: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation)، و[New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship)، و[Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)، و[Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

لإنشاء نهج مشاركة، استخدم [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). [لتطبيق نهج مشاركة على صندوق بريد أو مستخدم](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)، يلزم استخدام مجموعة تتألف من  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) و[Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) مع النهج المُنشأ حديثاً. [لتعديل نهج المشاركة أو تعطيله أو إزالته](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)، يلزم استخدام  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) و[Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**للتوصل إلى فهم كامل لهذا الموضوع، رجاءً اقرأ:**

[المشاركة في Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)