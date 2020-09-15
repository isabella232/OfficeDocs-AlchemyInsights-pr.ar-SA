---
title: تجاوز ساحة الانتظار
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684937"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="0938e-102">التحكم في إعدادات الانتظار ومستوي المشاركة في الفرق</span><span class="sxs-lookup"><span data-stu-id="0938e-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="0938e-103">إذا أردت السماح للجميع بما في ذلك ، بما في ذلك المستخدمين الذين لديهم طلب ، وخارجي ، ومجهول ، **لتجاوز ساحة الانتظار**، فاستخدم PowerShell لإنجاز هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="0938e-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="0938e-104">اليك مثال حول تعديل نهج الاجتماع العام لمؤسسك.</span><span class="sxs-lookup"><span data-stu-id="0938e-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="0938e-105">يتطلب أمر cmdlet هذا حاليا استخدام الوحدة النمطية ل PowerShell ل business.</span><span class="sxs-lookup"><span data-stu-id="0938e-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="0938e-106">للحصول علي اعداد لاستخدام أمر cmdlet هذا ، راجع [أداره النهج عبر PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="0938e-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="0938e-107">بمجرد اعداد نهج ، يجب تطبيقه علي المستخدمين ؛ أو ، إذا قمت بتعديل النهج العام ، سيتم تطبيقه علي المستخدمين تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="0938e-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="0938e-108">لأي تغيير في النهج ، ستحتاج إلى الانتظار لمده **4 ساعات** علي الأقل حتى 24 ساعة حتى تصبح النهج ساريه المفعول.</span><span class="sxs-lookup"><span data-stu-id="0938e-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="0938e-109">تاكد من مراجعه الوثائق أدناه قبل اجراء هذه التغييرات لفهم ما يسمح به بالبالضبط.</span><span class="sxs-lookup"><span data-stu-id="0938e-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="0938e-110">التعرف علي عناصر تحكم نهج ساحة انتظار اجتماعات الفرق</span><span class="sxs-lookup"><span data-stu-id="0938e-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="0938e-111">تتحكم هذه الإعدادات في المشاركين في الاجتماع في ساحة الانتظار قبل السماح لهم بالاجتماع ومستوي المشاركة المسموح به في اجتماع.</span><span class="sxs-lookup"><span data-stu-id="0938e-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="0938e-112">يمكنك استخدام PowerShell لتحديث إعدادات نهج الاجتماع الذي لم يتم تطبيقه بعد (المسمي "قريبا") في مركز أداره الفرق.</span><span class="sxs-lookup"><span data-stu-id="0938e-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="0938e-113">انظر أدناه للاطلاع علي مثال ل PowerShell cmdlet الذي يسمح لكل المستخدمين بتجاوز ساحة الانتظار.</span><span class="sxs-lookup"><span data-stu-id="0938e-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="0938e-114">ان الوصول [إلى الأشخاص تلقائيا](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) هو نهج لكل منظم والذي يتحكم ما إذا كان الأشخاص ينضمون إلى اجتماع مباشره أو تنتظر في ساحة الانتظار حتى يتم السماح لهم بالإقرار بالمستخدمين المصادق عليهم.</span><span class="sxs-lookup"><span data-stu-id="0938e-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="0938e-115">[السماح للأشخاص المجهولين ببدء الاجتماع](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) هو نهج لكل منظم والذي يتحكم في ما إذا كان الأشخاص المجهولين ، بما في ذلك المستخدمون من المؤسسات المتحدة الخاصة بالB2B</span><span class="sxs-lookup"><span data-stu-id="0938e-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="0938e-116">[السماح لمستخدمي الطلب بتجاوز ساحة الانتظار](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(** قريبا) هو نهج لكل منظم الذي يتحكم بما إذا كان الأشخاص الذين يقومون بالاتصال عبر الهاتف ، انضمون إلى الاجتماع مباشره أو انتظر في ساحة الانتظار بغض النظر عن الاعداد الذي يقوم به **الأشخاص بالدخول** .</span><span class="sxs-lookup"><span data-stu-id="0938e-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="0938e-117">[السماح لمنظمي بتجاوز إعدادات الانتظار](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(** القريبة) هو نهج لكل منظم والذي يتحكم في ما إذا كان منظم الاجتماع قد تجاوز إعدادات الانتظار التي قام المسؤول بتعيينها في العمل **تلقائيا** والسماح **لمستخدمي الطلب بتجاوز ساحة الانتظار** عند جدوله اجتماع جديد.</span><span class="sxs-lookup"><span data-stu-id="0938e-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="0938e-118">**ملاحظه:** أقرا [أداره نهج الاجتماع في فرق](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) للحصول علي نظره عامه حول نهج اجتماعات فرق Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0938e-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
