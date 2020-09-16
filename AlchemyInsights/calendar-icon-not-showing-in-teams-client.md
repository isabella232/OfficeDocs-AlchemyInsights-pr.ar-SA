---
title: عدم ظهور أيقونة "التقويم" في عميل Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: f30cd5bda62756cf6b912ed150b4e59e7ca4d85d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684685"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="9d948-102">عدم ظهور أيقونة "التقويم" في عميل Teams</span><span class="sxs-lookup"><span data-stu-id="9d948-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="9d948-103">تتطلب علامة تبويب "التقويم" في Teams إمكانية الوصول إلى علبة بريد Exchange عبر خدمات الويب من Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d948-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="9d948-104">يمكن أن تكون علبة بريد Exchange عبر الإنترنت أو محلية.</span><span class="sxs-lookup"><span data-stu-id="9d948-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="9d948-105">بالنسبة للمستخدمين عبر الإنترنت الذين لا يمكنهم رؤية علامة تبويب "التقويم"، تأكد من أنهم [لديهم رخصة علبة بريد Exchange Online وأن علبة البريد ممكّنة](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="9d948-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="9d948-106">إذا كان لدى المستخدم علبة بريد صالحة في Exchange Online، ولكن لا يزال يتعذر عليه رؤية علامة تبويب "التقويم"، فقد تكون المشكلة في الشبكة.</span><span class="sxs-lookup"><span data-stu-id="9d948-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="9d948-107">استخدم [محلل الاتصال عن بُعد من Microsoft](https://testconnectivity.microsoft.com/) وقم بتشغيل **اختبارات اتصال خدمات الويب من Microsoft Exchange** للمستخدمين المتأثرين.</span><span class="sxs-lookup"><span data-stu-id="9d948-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="9d948-108">وأخيراً يمكنك التحقق من [تطبيقات Teams – نُهج إعداد التطبيقات](https://admin.teams.microsoft.com/policies/app-setup) للتأكد من أنه لم تتم إزالة تطبيق التقويم من النهج الذي تم تطبيقه على المستخدم (على الأرجح **العمومي (افتراضي على مستوى المؤسسة)**.</span><span class="sxs-lookup"><span data-stu-id="9d948-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="9d948-109">إذا كان المستخدمون يعملون في الأساس محلياً، فأنت بحاجة إلى التأكد من أن "التكوين المختلط" سليم.</span><span class="sxs-lookup"><span data-stu-id="9d948-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="9d948-110">استخدم["معالج التكوين المختلط"](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)لاستكشاف الأخطاء وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="9d948-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="9d948-111">تجدر الإشارة إلى أن [Teams يتطلب Exchange 2016 CU3 أو إصدار أحدث](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="9d948-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
