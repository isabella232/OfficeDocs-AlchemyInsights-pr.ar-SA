---
title: 1490-troubleshooting-eDiscovery-failures
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 7b819b9bb18b5c0a635e708eccc0f23271267874707e5f3a7d41b633a05f2822
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105555"
---
# <a name="troubleshoot-content-search-errors"></a>استكشاف أخطاء البحث في المحتوى وإصلاحها

هل تواجه مشاكل في "البحث في المحتوى" أو تواجه حالات فشل عند تصدير نتائج البحث؟

على سبيل المثال، هل تتلقى ما يلي عند تشغيل عمليات البحث؟

- أخطاء CS008 أو CS012

- أخطاء انشغال الخادم/ينتهى

- حدث خطأ في التطبيق

أو عند البحث عن نتائج أو تصديرها من عدد كبير من علب البريد (أكثر من 100000 علبة بريد)، هل تظهر لك أخطاء في التصدير؟

بالنسبة إلى هذه الأنواع من الأخطاء، ا إعادة محاولة البحث عن مواقع المحتوى التي فشلت. راجع  [هذه المقالة](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) للحصول على مزيد من المعلومات.

إذا كنت تقوم بتصدير أكثر من 100 ألف علبة بريد، ستحتاج إلى استخدام Powershell التالي لتنزيل نتائج التصدير: تصدير النتائج من أكثر من  [100 ألف](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)علبة بريد .
