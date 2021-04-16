---
title: أداة تصدير eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814575"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>هل لا يمكنك تثبيت أداة تصدير eDiscovery أو تشغيلها؟

إذا لم تتمكن من تثبيت أداة تصدير eDiscovery أو تشغيلها لتنزيل نتائج البحث، فتحقق من الأمور التالية:
  
- يلبي الكمبيوتر الذي تستخدمه هذه المتطلبات الأساسية:

  - الإصدارات 32- أو 64 بت من Windows 7 والإصدارات الأحدث

  - Microsoft .NET Framework 4.7

  - مستعرض معتمد:

  - Microsoft Edge

    أو

  - Internet Explorer 10 والإصدارات الأحدث

    المستعرضات الأخرى، مثل Google Chrome و Mozilla Firefox غير معتمدة.

- يمكن لمنظمتك الاتصال بنقطة النهاية في Azure، **\* وهي .blob.core.windows.net** (يمثل أحرف البدل معرفا فريدا لمهمة التصدير).

- تم تعيين دور التصدير في مركز التوافق الأمني ل Microsoft 365. &amp; بشكل افتراضي، يتم تعيين هذا الدور إلى مجموعة دور eDiscovery Manager فقط. راجع [تعيين أذونات eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

لمزيد من المعلومات، راجع [تصدير نتائج البحث في المحتوى](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

إذا كنت تقوم بتصدير أكثر من 100 ألف علبة بريد، ستحتاج إلى استخدام Powershell التالي لتنزيل نتائج التصدير: تصدير النتائج من أكثر من  [100 ألف](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)علبة بريد .