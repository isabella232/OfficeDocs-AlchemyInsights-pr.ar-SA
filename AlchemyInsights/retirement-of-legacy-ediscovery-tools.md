---
title: تقاعد أدوات eDiscovery القديمة
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798536"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>تقاعد أدوات eDiscovery القديمة

نتيجة لوظائف eDiscovery الجديدة والمحسنة في مركز التوافق ل Microsoft 365، سيتم في الأشهر القادمة إعزال أدوات eDiscovery والأوامر القديمة التالية:

- [يتم وضع eDiscovery والمواعيد](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [في](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) مكانها في مركز إدارة Exchange.

- Cmdlets في Exchange Online PowerShell التي تدعم In-Place eDiscovery In-Place المواعيد. (يتم تعريف cmdlets هذه بشكل جماعي على أنها cmdlets *-MailboxSearch.) يشمل ذلك cmdlets التالية:

    - [البحث عن علبة بريد جديدة](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- الأمر [cmdlet "البحث في علبة](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) البريد" في Exchange Online PowerShell.
- العمليات التالية في API ل Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [eDiscovery المتقدم v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**المخطط الزمني للتقاعد**:
- **1 يوليو 2020** لم يعد بإمكانك إنشاء عمليات بحث وعمليات حفظ جديدة، ولكن يمكنك تشغيل عمليات البحث الموجودة وتحريرها وحذفها على حسابك الخاص. لم يعد دعم Microsoft يدعم In-Place eDiscovery & في EAC.
    
- 1 أكتوبر **2020** In-Place eDiscovery & سيتم وضع وظائف "المواضع الموضعية" في EAC في وضع القراءة فقط، بحيث يمكنك إزالة عمليات البحث والمواضع الموضعية الموجودة فقط.

**لمزيد من المعلومات، راجع:**

 - [ترحيل عمليات بحث eDiscovery القديمة والمحتجزة إلى مركز التوافق في Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [تقاعد أدوات eDiscovery القديمة](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [الأسئلة والأسئلة In-Place eDiscovery In-Place المواعيد](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



