---
title: تقاعد أدوات eDiscovery القديمة
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
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902607"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>تقاعد أدوات eDiscovery القديمة

نتيجة لوجود وظيفة eDiscovery الجديدة والمحسنة في مركز توافق Microsoft 365 ، سيتم إيقاف أدوات eDiscovery القديمة التالية والكوماندليتس في الأشهر القادمة:

- [وضع eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) الموضعي [والتعليق الموضعي](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) في مركز أداره Exchange.

- أوامر cmdlets في Exchange Online PowerShell التي تدعم قوائم eDiscovery الموضعية والموضعية. (يتم تعريف كل أوامر cmdlets التالية ك *-مايلبوكسسيرتش cmdlets). يتضمن هذا الاجراء أوامر cmdlets التالية:

    - [جديد-ميلبوكسسيرتش](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [تاريخ البدء ميلبوكسسيرتش](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [إيقاف الميلبوكسسيرتش](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [ميلبوكسسيرتش](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [البحث-علبه البريد](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) Cmdlet في Exchange Online PowerShell.
- العمليات التالية في واجهه برمجه تطبيقات Exchange Web Services:
    - [جيتسيرتشابليميلبوكسيس](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [سيثولدونمايلبوكسيس](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [جيثولدونمايلبوكسيس](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [EDiscovery المتقدمة v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**الخط الزمني لتقاعد المدة**:
- **1 يوليو 2020** لم يعد بإمكانك إنشاء عمليات بحث وقوائم احتجاز جديده ، ولكن يمكنك تشغيل عمليات البحث الموجودة وتحريرها وحذفها علي مسؤوليتك الخاصة. لم يعد دعم Microsoft أكثر دعما في وضع eDiscovery الموضعي & القوائم في EAC.
    
- **1 أكتوبر 2020** سيتم وضع وظيفة الوظائف الاضافيه لقوائم الاحتجاز في ال& مكان في القائمة المنسدلة في وضع القراءة فقط ، التالي يمكنك فقط أزاله عمليات البحث والقوائم الموجودة.

**لمزيد من المعلومات ، راجع**:

 - [ترحيل عمليات بحث eDiscovery القديمة وقوائم الاحتجاز إلى مركز توافق Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [تقاعد أدوات eDiscovery القديمة](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [اسئله حول eDiscovery الموضعي والتعليقات الموضعية](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



