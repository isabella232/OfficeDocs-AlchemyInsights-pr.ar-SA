---
title: CDN المستخدم لتشغيل الفيديو
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002552"
- "5146"
ms.openlocfilehash: c40606df4a79fed1e526440f7f27f8f15dbd2032
ms.sourcegitcommit: a98b25fa3cac9ebba983f4932881d774880aca93
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/13/2020
ms.locfileid: "44058847"
---
# <a name="cdn-used-for-video-playback"></a><span data-ttu-id="345cc-102">CDN المستخدم لتشغيل الفيديو</span><span class="sxs-lookup"><span data-stu-id="345cc-102">CDN used for video playback</span></span>

<span data-ttu-id="345cc-103">ستستخدم الأحداث المباشرة من Stream والتطبيق الخارجي أو الأحداث المباشرة للجهاز من Yammer/Teams لـ Azure CDN تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="345cc-103">Live events from Stream and External app or device live events from Yammer/Teams will automatically use Azure CDN.</span></span> <span data-ttu-id="345cc-104">مقاطع الفيديو التي تم تحميلها حسب الطلب لا تستخدم Azure CDN للتشغيل بعد.</span><span class="sxs-lookup"><span data-stu-id="345cc-104">On-demand videos uploaded to Stream don't yet use Azure CDN for playback.</span></span> <span data-ttu-id="345cc-105">يتم تشغيل ملفات الفيديو غير المباشرة في Stream من ملقم الأصل لخدمات وسائط Azure المقترنة بالمستأجر في منطقته الجغرافية.</span><span class="sxs-lookup"><span data-stu-id="345cc-105">Non-live videos in Stream are played back from the Azure Media Services origin server associated with your tenant in your tenant's geographic region.</span></span> <span data-ttu-id="345cc-106">لمزيد من المعلومات، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="345cc-106">For more information, see:</span></span>

- [<span data-ttu-id="345cc-107">CDN المستخدم لتشغيل الفيديو</span><span class="sxs-lookup"><span data-stu-id="345cc-107">CDN used for video playback</span></span>](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
