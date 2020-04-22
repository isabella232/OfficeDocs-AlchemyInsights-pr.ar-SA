---
title: التقاعد من أدوات eDiscovery تراث
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650555"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>التقاعد من أدوات eDiscovery تراث

نتيجة لوظيفة eDiscovery الجديدة والمحسنة في مركز Microsoft 365 Compliance، سيتم سحب أدوات وأوامر eDiscovery القديمة التالية في الأشهر المقبلة:

- [في مكان eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) وفي [مكان يحمل](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) في مركز إدارة Exchange.

- cmdlets PowerShell تبادل عبر الإنترنت التي تدعم في مكان eDiscovery وفي مكان يحمل. (يتم تعريف هذه cmdlets بشكل جماعي على أنها cmdlets *-MailboxSearch.) وهذا يشمل cmdlets التالية:

    - [بحث علبة بريد جديدة](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [بدء-علبة بريدالبحث](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [إيقاف علبة البريدالبحث](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [تعيين صندوق بريد البحث](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [cmdlet البحث علبة البريد](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) في تبادل PowerShell عبر الإنترنت.
- العمليات التالية في واجهة برمجة تطبيقات خدمات ويب Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [متقدمة eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**الجدول الزمني للتقاعد:**
- 1 أبريل 2020: لن تتمكن من إنشاء عمليات بحث جديدة وعمليات التحمل، ولكن لا يزال بإمكانك تشغيل عمليات البحث الحالية وتعديلها وحذفها على مسؤوليتك الخاصة. لن يدعم دعم Microsoft بعد الآن في مكان eDiscovery & يحمل في EAC.

- 1 يوليو 2020: سيتم وضع وظيفة eDiscovery & في مكان هاوية في EAC في وضع القراءة فقط. وهذا يعني أنك لن تتمكن إلا من إزالة عمليات البحث الحالية وعمليات الرفع.

**لمزيد من المعلومات، راجع:**

 - [ترحيل عمليات البحث القديمة eDiscovery وتحتجز إلى مركز الامتثال Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [التقاعد من أدوات eDiscovery القديمة](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [الأسئلة الشائعة حول eDiscovery في مكان ويحمل في مكان](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



