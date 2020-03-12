---
title: التقاعد من أدوات eDiscovery القديمة
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
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600337"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>التقاعد من أدوات eDiscovery القديمة

نتيجة لوظائف eDiscovery الجديدة والمحسنة في مركز الامتثال Microsoft 365، سيتم سحب أدوات eDiscovery القديمة التالية والأوامر في الأشهر المقبلة:

- [في مكان eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) وفي [مكان يحمل](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) في مركز إدارة Exchange.

- Cmdlets PowerShell Exchange عبر الإنترنت التي تدعم eDiscovery في المكان ويحمل في المكان. (يتم تعريف هذه cmdlets بشكل جماعي كـ *-MailboxSearch cmdlets.) وهذا يشمل cmdlets التالية:

    - [بحث جديد في علب ة البريد](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [بدء البحث في علبة البريد](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [إيقاف علبة البريد البحث](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [تعيين علبة البريد البحث](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [cmdlet البحث علبة البريد](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) في PowerShell تبادل عبر الإنترنت.
- العمليات التالية في API خدمات ويب Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 eDiscovery متقدم v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**الجدول الزمني للتقاعد:**
- 1 أبريل 2020: لن تتمكن من إنشاء عمليات بحث والاحتفاظ جديدة، ولكن لا يزال بإمكانك تشغيل عمليات البحث الحالية وتعديلها وحذفها على مسؤوليتك الخاصة. لن يدعم دعم Microsoft بعد الآن & في EـDiscovery في EAC.

- 1 يوليو 2020: سيتم وضع وظيفة eDiscovery & في EWHATفي EDISCOVERy في EAC في وضع القراءة فقط. وهذا يعني أنك ستتمكن فقط من إزالة عمليات البحث وقائمة.

**لمزيد من المعلومات، راجع:**

 - [ترحيل عمليات البحث عن eDiscovery القديمة وإمكانية حملها إلى مركز الامتثال Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [التقاعد من أدوات eDiscovery القديمة](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [الأسئلة الشائعة حول eDiscovery في المكان ويحمل في مكان](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



