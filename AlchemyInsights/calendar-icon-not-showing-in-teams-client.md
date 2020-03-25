---
title: عدم ظهور أيقونة "التقويم" في عميل Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931778"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="47c71-102">عدم ظهور أيقونة "التقويم" في عميل Teams</span><span class="sxs-lookup"><span data-stu-id="47c71-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="47c71-103">تتطلب علامة تبويب "التقويم" في Teams إمكانية الوصول إلى علبة بريد Exchange عبر خدمات الويب من Exchange.</span><span class="sxs-lookup"><span data-stu-id="47c71-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="47c71-104">يمكن أن تكون علبة بريد Exchange عبر الإنترنت أو محلية.</span><span class="sxs-lookup"><span data-stu-id="47c71-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="47c71-105">بالنسبة للمستخدمين عبر الإنترنت الذين لا يمكنهم رؤية علامة تبويب "التقويم"، تأكد من أنهم [لديهم رخصة علبة بريد Exchange Online وأن علبة البريد ممكّنة](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="47c71-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="47c71-106">إذا كان لدى المستخدم علبة بريد صالحة في Exchange Online، ولكن لا يزال يتعذر عليه رؤية علامة تبويب "التقويم"، فقد تكون المشكلة في الشبكة.</span><span class="sxs-lookup"><span data-stu-id="47c71-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="47c71-107">استخدم [محلل الاتصال عن بُعد من Microsoft](https://testconnectivity.microsoft.com/) وقم بتشغيل **اختبارات اتصال خدمات الويب من Microsoft Exchange** للمستخدمين المتأثرين.</span><span class="sxs-lookup"><span data-stu-id="47c71-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="47c71-108">وأخيراً يمكنك التحقق من [تطبيقات Teams – نُهج إعداد التطبيقات](https://admin.teams.microsoft.com/policies/app-setup) للتأكد من أنه لم تتم إزالة تطبيق التقويم من النهج الذي تم تطبيقه على المستخدم (على الأرجح **العمومي (افتراضي على مستوى المؤسسة)**.</span><span class="sxs-lookup"><span data-stu-id="47c71-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="47c71-109">إذا كان المستخدمون يعملون في الأساس محلياً، فأنت بحاجة إلى التأكد من أن "التكوين المختلط" سليم.</span><span class="sxs-lookup"><span data-stu-id="47c71-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="47c71-110">استخدم["معالج التكوين المختلط"](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)لاستكشاف الأخطاء وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="47c71-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="47c71-111">تجدر الإشارة إلى أن [Teams يتطلب Exchange 2016 CU3 أو إصدار أحدث](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="47c71-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
