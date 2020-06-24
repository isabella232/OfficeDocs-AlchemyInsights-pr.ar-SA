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
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>استخدام PowerShell لنُهج المشاركة وعلاقات المؤسسة


لعلاقات المؤسسة الرجاء مراجعة بناء الجملة التفصيلية ومعلومات المعلمة لـ: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation)، [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship)، [تعيين- المنظمةRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) [وإزالة-المنظمة.](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship)

لإنشاء نهج المشاركة استخدم [سياسة المشاركة الجديدة](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). [لتطبيق نهج مشاركة على علبة بريد أو مستخدم](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) تحتاج إلى استخدام تركيبة من علبة البريد [مجموعة](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) [وعلبة الحصول مع](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) النهج الذي تم إنشاؤه حديثاً. [لتعديل أو تعطيل أو إزالة نهج المشاركة](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) تحتاج إلى استخدام ["سياسة مشاركة Set-Sharing"](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) و ["إزالة-المشاركة السياسة](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**لفهم هذا الموضوع بشكل كامل يرجى قراءة:**

[المشاركة في Exchange عبر الإنترنت](https://docs.microsoft.com/exchange/sharing/sharing)