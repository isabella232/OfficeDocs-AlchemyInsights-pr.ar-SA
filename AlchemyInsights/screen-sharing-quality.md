---
title: جودة مشاركة الشاشة
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11061"
- "11062"
- "9002254"
- "9002536"
ms.openlocfilehash: 0832f886d3f5c0bfbfe138647403e4e215deaacb
ms.sourcegitcommit: d822377ec76adf9ef6d13bc761a16c9900a3e7cb
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/26/2021
ms.locfileid: "52124744"
---
# <a name="screen-sharing-quality"></a><span data-ttu-id="2ea05-102">جودة مشاركة الشاشة</span><span class="sxs-lookup"><span data-stu-id="2ea05-102">Screen sharing quality</span></span>

<span data-ttu-id="2ea05-103">في معظم الحالات، تنزل مشاكل الجودة في مشاركة الشاشة إلى نطاق ترددي محدود من جانب العميل.</span><span class="sxs-lookup"><span data-stu-id="2ea05-103">In most cases quality issues with Screen Sharing comes down to limited bandwidth from the client side.</span></span>  <span data-ttu-id="2ea05-104">عندما لا يكون النطاق الترددي محدودا، يعمل Teams على تحسين جودة الوسائط، بما في ذلك دقة فيديو تصل إلى 1080 p، وما يصل إلى 30fps للفيديو و15fps للمحتوى، والصوت عالي الدقة.</span><span class="sxs-lookup"><span data-stu-id="2ea05-104">Where bandwidth isn't limited, Teams optimizes media quality, including up to 1080p video resolution, up to 30fps for video and 15fps for content, and high-fidelity audio.</span></span>

<span data-ttu-id="2ea05-105">Teams دائما المحافظة على استخدام النطاق الترددي ويمكنه تقديم جودة فيديو عالية الدقة في أقل من 1.2Mbps.</span><span class="sxs-lookup"><span data-stu-id="2ea05-105">Teams is always conservative on bandwidth utilization and can deliver HD video quality in under 1.2Mbps.</span></span> <span data-ttu-id="2ea05-106">يختلف استهلاك النطاق الترددي الفعلي في كل مكالمة صوتية/فيديو أو اجتماع استنادا إلى عوامل مثل تخطيط الفيديو و دقة الفيديو وإطارات الفيديو في الثانية.</span><span class="sxs-lookup"><span data-stu-id="2ea05-106">The actual bandwidth consumption in each audio/video call or meeting vary based on factors such as video layout, video resolution, and video frames per second.</span></span> <span data-ttu-id="2ea05-107">عند توفر نطاق ترددي أكبر، تزيد الجودة والاستخدام لتقديم أفضل تجربة.</span><span class="sxs-lookup"><span data-stu-id="2ea05-107">When more bandwidth is available, quality and usage increase to deliver the best experience.</span></span> <span data-ttu-id="2ea05-108">يصف هذا الجدول كيفية استخدام Teams النطاق الترددي:</span><span class="sxs-lookup"><span data-stu-id="2ea05-108">This table describes how Teams uses bandwidth:</span></span>

<span data-ttu-id="2ea05-109">**سيناريوهات النطاق الترددي (لأعلى/أسفل)**</span><span class="sxs-lookup"><span data-stu-id="2ea05-109">**Bandwidth(up/down) Scenarios**</span></span>

- <span data-ttu-id="2ea05-110">30 كيلو يب الثانية للمكاتب الصوتي من نظير إلى نظير</span><span class="sxs-lookup"><span data-stu-id="2ea05-110">30 kbps Peer-to-peer audio calling</span></span>

- <span data-ttu-id="2ea05-111">130 كيلو في الثانية للمكاتب الصوتي من نظير إلى نظير ومشاركة الشاشة</span><span class="sxs-lookup"><span data-stu-id="2ea05-111">130 kbps Peer-to-peer audio calling and screen sharing</span></span>

- <span data-ttu-id="2ea05-112">مكالمة فيديو بجودة من نظير إلى نظير 500 كيلوبت في الثانية 360 p في 30fps</span><span class="sxs-lookup"><span data-stu-id="2ea05-112">500 kbps Peer-to-peer quality video calling 360p at 30fps</span></span>

- <span data-ttu-id="2ea05-113">1.2 Mbps في الثانية لمكاتب الفيديو عالية الجودة من نظير إلى نظير بدقة عالية 720 p بدقة 30fps</span><span class="sxs-lookup"><span data-stu-id="2ea05-113">1.2 Mbps Peer-to-peer HD quality video calling with resolution of HD 720p at 30fps</span></span>

- <span data-ttu-id="2ea05-114">1.5 Mbps في الثانية لمكاتب الفيديو عالية الجودة من نظير إلى نظير بدقة عالية 1080 p بدقة 30fps</span><span class="sxs-lookup"><span data-stu-id="2ea05-114">1.5 Mbps Peer-to-peer HD quality video calling with resolution of HD 1080p at 30fps</span></span>

- <span data-ttu-id="2ea05-115">مكالمة فيديو مجموعة 500kbps/1Mbps</span><span class="sxs-lookup"><span data-stu-id="2ea05-115">500kbps/1Mbps Group Video calling</span></span>

- <span data-ttu-id="2ea05-116">1Mbps/2Mbps مكالمة فيديو مجموعة عالية الدقة (مقاطع فيديو 540 p على شاشة 1080 p)</span><span class="sxs-lookup"><span data-stu-id="2ea05-116">1Mbps/2Mbps HD Group video calling (540p videos on 1080p screen)</span></span>

<span data-ttu-id="2ea05-117">لمزيد من المعلومات، راجع إعداد شبكة [مؤسستك Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span><span class="sxs-lookup"><span data-stu-id="2ea05-117">For more information, see [Prepare your organization's network for Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span></span>