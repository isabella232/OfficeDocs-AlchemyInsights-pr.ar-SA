---
title: استخدام منع التعقب في Microsoft Edge (Chromium)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8328"
- "9004625"
ms.openlocfilehash: 09e9a7303063328cd7bd0a0fcbf9629a3b38ebb5
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420681"
---
# <a name="use-tracking-prevention-in-microsoft-edge-chromium"></a><span data-ttu-id="70279-102">استخدام منع التعقب في Microsoft Edge (Chromium)</span><span class="sxs-lookup"><span data-stu-id="70279-102">Use tracking prevention in Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="70279-103">إن منع التعقب في Microsoft Edge يحد من قدرة المتعقب على الوصول إلى مساحة التخزين المستندة إلى المستعرض ونهاية الشبكة.</span><span class="sxs-lookup"><span data-stu-id="70279-103">Tracking prevention in Microsoft Edge limits a tracker's ability to access browser-based storage and the network.</span></span> <span data-ttu-id="70279-104">لقد تم تصميم هذه الميزة لدعم التزامنا بمساعدة المستخدمين في الحفاظ على أمانهم على الويب باستخدام Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="70279-104">The feature is built to uphold our commitment to helping users stay safe on the web with Microsoft Edge.</span></span> <span data-ttu-id="70279-105">لمزيد من المعلومات، راجع [منع التعقب في Microsoft Edge (Chromium)](https://go.microsoft.com/fwlink/?linkid=2135435) [ونعد بخصوصية المستعرض](https://go.microsoft.com/fwlink/?linkid=2135350).</span><span class="sxs-lookup"><span data-stu-id="70279-105">For more information, see [Tracking prevention in Microsoft Edge (Chromium)](https://go.microsoft.com/fwlink/?linkid=2135435) and [Our browser privacy promise](https://go.microsoft.com/fwlink/?linkid=2135350).</span></span>

<span data-ttu-id="70279-106">يوفر Microsoft Edge ثلاثة مستويات لمنع التعقب (يمكن تحديدها في edge://settings/privacy):</span><span class="sxs-lookup"><span data-stu-id="70279-106">Microsoft Edge offers three levels of tracking prevention (they can be selected in edge://settings/privacy):</span></span>

- <span data-ttu-id="70279-107">**Basic** هو الأقل تقييدا وتصميما للمستخدمين الذين يستمتعون بالإعلانات المخصصة ولا يمانعون في تعقبهم على الويب.</span><span class="sxs-lookup"><span data-stu-id="70279-107">**Basic** is the least restrictive and designed for users who enjoy personalized advertisements and don't mind being tracked on the web.</span></span> <span data-ttu-id="70279-108">تحمي الأساسي المستخدمين فقط من أجهزة التعقب الضارة، مثل بصمات الأصابع والمتشفرات.</span><span class="sxs-lookup"><span data-stu-id="70279-108">Basic protects users only against malicious trackers, such as fingerprinters and cryptominers.</span></span>
- <span data-ttu-id="70279-109">**المتوازن** هو المستوى الافتراضي وقد تم تصميمه للمستخدمين الذين يرغبون في رؤية إعلانات أقل تتابعهم عبر الويب.</span><span class="sxs-lookup"><span data-stu-id="70279-109">**Balanced** is the default level and designed for users who want to see fewer advertisements that follow them around the web.</span></span> <span data-ttu-id="70279-110">لا يهدف المستوى المتوازن إلى حظر متعقبات المواقع التي لا يتفاعل معها المستخدمون فحسب، بل أيضا لتقليل مخاطر مشاكل التوافق.</span><span class="sxs-lookup"><span data-stu-id="70279-110">Balanced level aims not only to block trackers from sites that users never engage with but also to minimize the risk of compatibility issues.</span></span>
- <span data-ttu-id="70279-111">**التقيد** هو الأكثر تقييدا وقد تم تصميمه للمستخدمين الذين لا يمانعون في المضحية بتوافق موقع ويب للحصول على أقصى قدر من الخصوصية.</span><span class="sxs-lookup"><span data-stu-id="70279-111">**Strict** is the most restrictive and designed for users who don't mind sacrificing website compatibility for maximum privacy.</span></span>