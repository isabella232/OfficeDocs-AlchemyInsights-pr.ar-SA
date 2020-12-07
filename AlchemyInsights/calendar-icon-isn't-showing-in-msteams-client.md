---
title: أيقونه التقويم لا تظهر في عميل فرق Microsoft
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583170"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="66b22-102">أيقونه التقويم لا تظهر في عميل فرق Microsoft</span><span class="sxs-lookup"><span data-stu-id="66b22-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="66b22-103">تتطلب علامة التبويب " **التقويم** " في الفرق الوصول إلى علبه بريد Exchange عبر خدمات exchange علي الويب.</span><span class="sxs-lookup"><span data-stu-id="66b22-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="66b22-104">يمكن ان تكون علبه بريد Exchange متصلة أو محليه.</span><span class="sxs-lookup"><span data-stu-id="66b22-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="66b22-105">بالنسبة للمستخدمين المتصلين الذين لا يريون علامة التبويب " **التقويم** " ، تاكد من [انه مرخص لك بالنسبة إلى علبه بريد Exchange Online ومن ان علبه البريد ممكنة](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="66b22-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="66b22-106">إذا كان المستخدمون يستخدم محليا ، ستحتاج إلى التاكد من ان التكوين المختلط سليم.</span><span class="sxs-lookup"><span data-stu-id="66b22-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="66b22-107">استخدم["معالج التكوين المختلط"](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)لاستكشاف الأخطاء وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="66b22-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="66b22-108">تجدر الإشارة إلى أن [Teams يتطلب Exchange 2016 CU3 أو إصدار أحدث](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="66b22-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="66b22-109">للحصول علي مزيد من المعلومات وخطوات استكشاف الأخطاء وإصلاحها ، راجع [استكشاف أخطاء فرق Microsoft ومشاكل التفاعل مع خادم Exchange](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span><span class="sxs-lookup"><span data-stu-id="66b22-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
