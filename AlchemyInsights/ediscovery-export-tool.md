---
title: أداه تصدير eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277953"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>هل يتعذر عليك تثبيت أداه تصدير eDiscovery أو تشغيلها ؟

إذا تعذر عليك تثبيت أداه تصدير eDiscovery أو تشغيلها لتنزيل نتائج البحث ، فتحقق من الأمور التالية:
  
- يلبي الكمبيوتر الذي تستخدمه هذه المتطلبات التجريبية:

  - الإصدارات 32 أو 64 بت لنظام التشغيل Windows 7 والإصدارات الأحدث

  - Microsoft .NET Framework 4.7

  - مستعرض معتمد:

  - Microsoft Edge

    Or

  - Internet Explorer 10 والإصدارات الأحدث

    لا يتم دعم المستعرضات الأخرى ، مثل Google Chrome و Mozilla Firefox.

- يمكن لمؤسسك الاتصال بنقطه النهاية في Azure ، وهو عبارة عن ** \* blob.core.windows.net** (يمثل حرف البدل معرفا فريدا لمهمة التصدير).

- لقد قمت بتعيين دور التصدير في مركز توافق الأمان ل Microsoft 365 &amp; . بشكل افتراضي ، يتم تعيين هذا الدور فقط إلى مجموعه ادوار أداره eDiscovery. راجع [تعيين أذونات eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

للحصول علي مزيد من المعلومات ، راجع [تصدير نتائج البحث في المحتوي](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

إذا كنت تقوم بتصدير أكثر من 100 كيلوبايت ، ستحتاج إلى استخدام Powershell التالي لتنزيل نتائج التصدير:  [تصدير النتائج من أكثر من 100 كيلوبايت علبه بريد](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).