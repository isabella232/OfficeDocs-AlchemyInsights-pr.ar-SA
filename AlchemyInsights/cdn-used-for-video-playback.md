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
# <a name="cdn-used-for-video-playback"></a><span data-ttu-id="0fde3-102">CDN المستخدم لتشغيل الفيديو</span><span class="sxs-lookup"><span data-stu-id="0fde3-102">CDN used for video playback</span></span>

<span data-ttu-id="0fde3-103">ستستخدم الأحداث المباشرة من Stream والتطبيق الخارجي أو الأحداث المباشرة للجهاز من Yammer/Teams لـ Azure CDN تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="0fde3-103">Live events from Stream and External app or device live events from Yammer/Teams will automatically use Azure CDN.</span></span> <span data-ttu-id="0fde3-104">مقاطع الفيديو التي تم تحميلها حسب الطلب لا تستخدم Azure CDN للتشغيل بعد.</span><span class="sxs-lookup"><span data-stu-id="0fde3-104">On-demand videos uploaded to Stream don't yet use Azure CDN for playback.</span></span> <span data-ttu-id="0fde3-105">يتم تشغيل ملفات الفيديو غير المباشرة في Stream من ملقم الأصل لخدمات وسائط Azure المقترنة بالمستأجر في منطقته الجغرافية.</span><span class="sxs-lookup"><span data-stu-id="0fde3-105">Non-live videos in Stream are played back from the Azure Media Services origin server associated with your tenant in your tenant's geographic region.</span></span> <span data-ttu-id="0fde3-106">لمزيد من المعلومات، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="0fde3-106">For more information, see:</span></span>

- [<span data-ttu-id="0fde3-107">CDN المستخدم لتشغيل الفيديو</span><span class="sxs-lookup"><span data-stu-id="0fde3-107">CDN used for video playback</span></span>](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
