---
title: 1490-استكشاف الأخطاء وإصلاحها-eDiscovery-فشل
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
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277826"
---
# <a name="troubleshoot-content-search-errors"></a>استكشاف أخطاء البحث في المحتوي وإصلاحها

هل تواجه مشاكل في البحث عن المحتوي أو الحصول علي حالات الفشل عند تصدير نتائج البحث ؟

علي سبيل المثال ، يمكنك تلقي ما يلي عند تشغيل عمليات البحث ؟

- أخطاء CS008 أو CS012

- أخطاء مشغولة/مهله الخادم

- حدث خطا في التطبيق

أو عند البحث أو التصدير من عدد كبير من علب البريد (عبر علب بريد 100,000) ، هل تحصل علي أخطاء التصدير ؟

بالنسبة إلى هذه الأنواع من الأخطاء ، أعد محاولة البحث عن مواقع المحتوي التي فشلت. راجع  [هذه المقالة](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) للحصول علي مزيد من المعلومات.

إذا كنت تقوم بتصدير أكثر من 100 كيلوبايت ، ستحتاج إلى استخدام Powershell التالي لتنزيل نتائج التصدير:  [تصدير النتائج من أكثر من 100 كيلوبايت علبه بريد](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
