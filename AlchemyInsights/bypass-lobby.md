---
title: الردهة التفافيه
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889069"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="79e91-102">ضبط إعدادات اللوبي ومستوي المشاركة في الفرق</span><span class="sxs-lookup"><span data-stu-id="79e91-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="79e91-103">إذا كنت ترغب في السماح للجميع ، بما في ذلك المستخدمين الهاتفيين والخارجيين والمجهولين ، **بتجاوز اللوبي**، فاستخدم PowerShell لإنجاز هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="79e91-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="79e91-104">في ما يلي مثال علي تعديل نهج الاجتماعات العمومية للمؤسسة الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="79e91-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="79e91-105">يتطلب هذا cmdlet حاليا استخدام سكايب للوحدة النمطية PowerShell الاعمال.</span><span class="sxs-lookup"><span data-stu-id="79e91-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="79e91-106">للحصول علي اعداد لاستخدام هذا cmdlet ، تحقق من [أداره السياسات عبر PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="79e91-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="79e91-107">بمجرد اعداد سياسة ، تحتاج إلى تطبيقها علي المستخدمين. أو ، إذا قمت بتعديل النهج العمومي ، سيتم تطبيقه تلقائيا علي المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="79e91-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="79e91-108">بالنسبة لأي تغيير في السياسة ، تحتاج إلى الانتظار لمده **4 ساعات علي الأقل حتى 24 ساعة حتى** تسري السياسات.</span><span class="sxs-lookup"><span data-stu-id="79e91-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="79e91-109">تاكد من مراجعه الوثائق أدناه قبل اجراء هذه التغييرات لفهم ما يسمح به هذا بالبالضبط.</span><span class="sxs-lookup"><span data-stu-id="79e91-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="79e91-110">فهم فرق التحكم في نهج اللوبي</span><span class="sxs-lookup"><span data-stu-id="79e91-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="79e91-111">تتحكم هذه الإعدادات في الاجتماعات التي ينتظرها المشاركون في الردهة قبل قبولهم في الاجتماع ومستوي المشاركة المسموح بها في الاجتماع.</span><span class="sxs-lookup"><span data-stu-id="79e91-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="79e91-112">يمكنك استخدام PowerShell لتحديث إعدادات نهج الاجتماع التي لم يتم تنفيذها بعد (المسمي "قريبا") في مركز أداره الفرق.</span><span class="sxs-lookup"><span data-stu-id="79e91-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="79e91-113">انظر أدناه للحصول علي مثال cmdlet PowerShell التي تسمح لجميع المستخدمين لتجاوز الردهة.</span><span class="sxs-lookup"><span data-stu-id="79e91-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="79e91-114">[القبول التلقائي للأشخاص](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) هو نهج لكل منظم يتحكم في ما إذا كان الأشخاص ينضمون إلى الاجتماع مباشره أو ينتظرون في الردهة حتى يتم قبولهم من قبل مستخدم مصادق عليه.</span><span class="sxs-lookup"><span data-stu-id="79e91-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="79e91-115">[السماح للأشخاص المجهولين ببدء اجتماع](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) هو نهج لكل منظم يتحكم في ما إذا كان بإمكان الأشخاص المجهولين ، بما في ذلك المستخدمين B2B والمتحدين ، الانضمام إلى اجتماع المستخدم بدون مستخدم مصادق عليه من المؤسسة في الحضور.</span><span class="sxs-lookup"><span data-stu-id="79e91-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="79e91-116">[السماح لمستخدمي الطلب الهاتفي بتجاوز الردهة](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**قريبا**) هو نهج لكل منظم يتحكم في ما إذا كان الأشخاص الذين يقومون بالاتصال بالهاتف بالانضمام إلى الاجتماع مباشره أو الانتظار في الردهة بغض النظر عن السماح **للأشخاص** بالاعداد تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="79e91-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="79e91-117">[السماح للمنظمين بتجاوز إعدادات اللوبي](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**قريبا**) هو نهج لكل منظم يتحكم في ما إذا كان منظم الاجتماع يمكنه تجاوز إعدادات الردهة التي يقوم المسؤول بتعيينها **تلقائيا** **والسماح لمستخدمي الطلب الهاتفي بتجاوز الردهة** عندما يقومون بجدوله اجتماع جديد.</span><span class="sxs-lookup"><span data-stu-id="79e91-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="79e91-118">**ملاحظه:** قراءه [أداره نهج الاجتماع في الفرق](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) للحصول علي نظره عامه كامله حول نهج اجتماع فرق Microsoft.</span><span class="sxs-lookup"><span data-stu-id="79e91-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
