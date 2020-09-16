---
title: تقاعد أدوات eDiscovery القديمة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727770"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>تقاعد أدوات eDiscovery القديمة

نتيجة لوجود وظيفة eDiscovery الجديدة والمحسنة في مركز توافق Microsoft 365 ، سيتم إيقاف أدوات eDiscovery القديمة التالية والكوماندليتس في الأشهر القادمة:

- [وضع eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) الموضعي [والتعليق الموضعي](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) في مركز أداره Exchange.

- أوامر cmdlets في Exchange Online PowerShell التي تدعم قوائم eDiscovery الموضعية والموضعية. (يتم تعريف كل أوامر cmdlets التالية ك *-مايلبوكسسيرتش cmdlets). يتضمن هذا الاجراء أوامر cmdlets التالية:

    - [جديد-مايلبوكسسيرتش](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [تاريخ البدء مايلبوكسسيرتش](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [إيقاف المايلبوكسسيرتش](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [مايلبوكسسيرتش](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [البحث-علبه البريد](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) Cmdlet في Exchange Online PowerShell.
- العمليات التالية في واجهه برمجه تطبيقات Exchange Web Services:
    - [جيتسيرتشابليمايلبوكسيس](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
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



