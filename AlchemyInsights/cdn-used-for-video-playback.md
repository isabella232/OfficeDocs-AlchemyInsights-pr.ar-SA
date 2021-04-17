---
title: CDN المستخدم لتشغيل الفيديو
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002552"
- "5146"
ms.openlocfilehash: d9c5f8f586e7f5aa079b28584375516ec8401ca7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819355"
---
# <a name="cdn-used-for-video-playback"></a>CDN المستخدم لتشغيل الفيديو

ستستخدم الأحداث المباشرة من Stream والتطبيق الخارجي أو الأحداث المباشرة للجهاز من Yammer/Teams لـ Azure CDN تلقائياً. مقاطع الفيديو التي تم تحميلها حسب الطلب لا تستخدم Azure CDN للتشغيل بعد. يتم تشغيل ملفات الفيديو غير المباشرة في Stream من ملقم الأصل لخدمات وسائط Azure المقترنة بالمستأجر في منطقته الجغرافية. لمزيد من المعلومات، اطلع على:

- [CDN المستخدم لتشغيل الفيديو](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
