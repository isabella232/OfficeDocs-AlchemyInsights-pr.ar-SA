---
title: تجاوز ساحة الانتظار
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820021"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="afee4-102">التحكم في إعدادات ساحة الانتظار ومستوى المشاركة في Teams</span><span class="sxs-lookup"><span data-stu-id="afee4-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="afee4-103">إذا كنت تريد السماح للجميع، بما في ذلك المستخدمين الذين يستخدمون الطلب الهاتفي والمستخدمين الخارجيين والمجهولين، بتجاوز ساحة الانتظار **،** فاستخدم PowerShell لتنفيذ هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="afee4-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="afee4-104">فيما يلي مثال لتعديل نهج الاجتماع العام لمنظمتك.</span><span class="sxs-lookup"><span data-stu-id="afee4-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="afee4-105">يتطلب الأمر cmdlet هذا حاليا استخدام وحدة Skype for Business PowerShell النمطية.</span><span class="sxs-lookup"><span data-stu-id="afee4-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="afee4-106">للحصول على إعداد لاستخدام الأمر cmdlet هذا، راجع [إدارة سياسات عبر PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="afee4-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="afee4-107">بعد إعداد نهج، ستحتاج إلى تطبيقه على المستخدمين؛ أو، إذا قمت بتعديل النهج العام، سيتم تطبيقه تلقائيا على المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="afee4-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="afee4-108">لأي تغيير في النهج، يجب الانتظار 4 ساعات على الأقل حتى **24 ساعة** حتى يتم تطبيق النهج.</span><span class="sxs-lookup"><span data-stu-id="afee4-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="afee4-109">تأكد من مراجعة الوثائق أدناه قبل إجراء هذه التغييرات لفهم ما يسمح به ذلك بالضبط.</span><span class="sxs-lookup"><span data-stu-id="afee4-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="afee4-110">فهم عناصر التحكم في نهج ساحة الانتظار لاجتماع Teams</span><span class="sxs-lookup"><span data-stu-id="afee4-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="afee4-111">تتحكم هذه الإعدادات بالمشاركين في الاجتماع الذين ينتظرون في ساحة الانتظار قبل أن يسمح لهم ب المشاركة في الاجتماع ومستوى المشاركة المسموح لهم به في الاجتماع.</span><span class="sxs-lookup"><span data-stu-id="afee4-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="afee4-112">يمكنك استخدام PowerShell لتحديث إعدادات نهج الاجتماع التي لم يتم تنفيذها بعد (المسمى "قريبا") في مركز إدارة Teams.</span><span class="sxs-lookup"><span data-stu-id="afee4-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="afee4-113">راجع أدناه للحصول على مثال PowerShell cmdlet الذي يسمح لجميع المستخدمين بتجاوز ساحة الانتظار.</span><span class="sxs-lookup"><span data-stu-id="afee4-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="afee4-114">[إن قبول الأشخاص](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) تلقائيا هو نهج لكل منظم يتحكم في انضمام الأشخاص إلى اجتماع مباشرة أو الانتظار في ساحة الانتظار حتى يتم قبولهم من قبل مستخدم مصدق عليه.</span><span class="sxs-lookup"><span data-stu-id="afee4-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="afee4-115">[](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) السماح للأشخاص المجهولين ببدء اجتماع هو نهج لكل منظم يتحكم في ما إذا كان يمكن للأشخاص المجهولين، بما في ذلك B2B والمستخدمين المتصلين، الانضمام إلى اجتماع المستخدم بدون مستخدم مصدق عليه من المؤسسة الحاضرة.</span><span class="sxs-lookup"><span data-stu-id="afee4-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="afee4-116">[](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) السماح لمستخدمي الطلب بتجاوز ساحة الانتظار (قريبا)هو نهج لكل منظم يتحكم في انضمام الأشخاص الذين يتصلون هاتفيا إلى الاجتماع مباشرة أو الانتظار في ساحة الانتظار بغض النظر عن إعداد السماح للأشخاص **تلقائيا.**</span><span class="sxs-lookup"><span data-stu-id="afee4-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="afee4-117">السماح للمنظمين بتجاوز إعدادات ساحة الانتظار [(قريبا)](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) هو نهج لكل منظم يتحكم في ما إذا كان يمكن لمنظم الاجتماع تجاوز  إعدادات ساحة الانتظار التي حددها المسؤول في السماح للأشخاص تلقائيا والسماح لمستخدمي الطلب بتجاوز ساحة الانتظار عند جدولة اجتماع جديد. </span><span class="sxs-lookup"><span data-stu-id="afee4-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="afee4-118">**ملاحظة:** اقرأ [إدارة سياسات الاجتماعات في Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) للحصول على نظرة عامة كاملة حول سياسات اجتماعات Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="afee4-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
