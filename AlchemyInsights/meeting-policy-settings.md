---
title: إعدادات نهج الاجتماع
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042831"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="cd1d6-102">إدارة نُهج الاجتماعات في Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="cd1d6-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="cd1d6-103">**ملاحظة: قد يستغرق الأمر ما يصل إلى 24 ساعة حتى تسري تغييرات النهج على المستخدمين.**</span><span class="sxs-lookup"><span data-stu-id="cd1d6-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="cd1d6-104">قد لا تتمكن من إجراء تغييرات على النُهج التي تم إنشاؤها حديثًا على الفور؛ انتظر 4 ساعات وحاول تعديل نهج تم إنشاؤه حديثًا مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="cd1d6-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="cd1d6-105">يتم استخدام نُهج الاجتماع للتحكم في الميزات المتوفرة للمشاركين في الاجتماع للاجتماعات المجدولة من قبل المستخدمين في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="cd1d6-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="cd1d6-106">قد لا يتم تنفيذ بعض ميزات نُهج الاجتماع في مركز إدارة الفرق حتى الآن (يتم تسمية هذه الميزات "قريبًا" في الوثائق).</span><span class="sxs-lookup"><span data-stu-id="cd1d6-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="cd1d6-107">في هذه الحالة، أو إذا كنت تحصل على خطأ مثل "لا يمكننا تحديث النهج الآن ولكن حاول مرة أخرى لاحقاً" في مركز إدارة Microsoft Teams، نوصي باستخدام PowerShell لإنشاء أو تعديل نُهج اجتماع الفرق.</span><span class="sxs-lookup"><span data-stu-id="cd1d6-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="cd1d6-108">لمزيد من المعلومات حول نُهج الاجتماع، راجع الموارد التالية:</span><span class="sxs-lookup"><span data-stu-id="cd1d6-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="cd1d6-109">للتعرف على كيفية إنشاء النُهج وإجراء التغييرات وتعيين المستخدمين إلى النهج، راجع [إدارة نُهج الاجتماع في الفرق](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="cd1d6-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="cd1d6-110">لإجراء تغييرات في السياسة باستخدام cmdlets PowerShell، راجع [نظرة عامة على Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="cd1d6-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="cd1d6-111">تحتاج إلى استخدام [وحدة Skype for Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) لسياسات اجتماع الفرق.</span><span class="sxs-lookup"><span data-stu-id="cd1d6-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="cd1d6-112">مراجعة [وثائق cmdlets \*CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) لمزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="cd1d6-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

