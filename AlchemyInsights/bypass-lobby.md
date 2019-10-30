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
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768427"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="574f3-102">ضبط إعدادات اللوبي ومستوي المشاركة</span><span class="sxs-lookup"><span data-stu-id="574f3-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="574f3-103">إذا كنت ترغب في السماح للجميع ، بما في ذلك المستخدمين الهاتفيين والخارجيين والمجهولين بتجاوز اللوبي في فرق Microsoft ، يمكنك استخدام PowerShell للقيام بذلك.</span><span class="sxs-lookup"><span data-stu-id="574f3-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby in Microsoft Teams, you can use PowerShell to do it.</span></span> <span data-ttu-id="574f3-104">في ما يلي مثال علي تعديل نهج الاجتماعات العمومية للمؤسسة الخاصة بك:</span><span class="sxs-lookup"><span data-stu-id="574f3-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="574f3-105">يتطلب هذا cmdlet حاليا استخدام سكايب للوحدة النمطية PowerShell الاعمال.</span><span class="sxs-lookup"><span data-stu-id="574f3-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="574f3-106">للحصول علي الاعداد لاستخدام هذا cmdlet ، تحقق من [أداره النهج عبر PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="574f3-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="574f3-107">يمكنك اعداد سياسة جديده ، والتي ستحتاج بعد ذلك إلى تطبيقها علي المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="574f3-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="574f3-108">إذا قمت بتعديل النهج العمومي سيتم تطبيقه تلقائيا علي المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="574f3-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="574f3-109">لأي تغيير في السياسة تحتاج إلى الانتظار 4 ساعات علي الأقل وتصل إلى 24 ساعة حتى تسري السياسات.</span><span class="sxs-lookup"><span data-stu-id="574f3-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="574f3-110">تاكد من مراجعه الوثائق أدناه قبل اجراء هذه التغييرات لفهم ما يسمح به هذا بالبالضبط.</span><span class="sxs-lookup"><span data-stu-id="574f3-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="574f3-111">فهم فرق التحكم في نهج اللوبي</span><span class="sxs-lookup"><span data-stu-id="574f3-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="574f3-112">[القبول التلقائي للأشخاص](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) هو نهج لكل منظم يتحكم في ما إذا كان الأشخاص ينضمون إلى الاجتماع مباشره أو ينتظرون في الردهة حتى يتم قبولهم من قبل مستخدم مصادق عليه.</span><span class="sxs-lookup"><span data-stu-id="574f3-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="574f3-113">[السماح للأشخاص المجهولين ببدء اجتماع](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) هو نهج لكل منظم يتحكم في ما إذا كان بإمكان الأشخاص المجهولين ، بما في ذلك المستخدمين B2B والمتحدين ، الانضمام إلى اجتماع المستخدم بدون مستخدم مصادق عليه من المؤسسة في الحضور.</span><span class="sxs-lookup"><span data-stu-id="574f3-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="574f3-114">[السماح لمستخدمي الطلب الهاتفي بتجاوز الردهة](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**قريبا**) هو نهج لكل منظم يتحكم في ما إذا كان الأشخاص الذين يقومون بالاتصال بالهاتف بالانضمام إلى الاجتماع مباشره أو الانتظار في الردهة بغض النظر عن السماح **للأشخاص** بالاعداد تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="574f3-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="574f3-115">[السماح للمنظمين بتجاوز إعدادات اللوبي](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**قريبا**) هو نهج لكل منظم يتحكم في ما إذا كان منظم الاجتماع يمكنه تجاوز إعدادات الردهة التي يقوم المسؤول بتعيينها **تلقائيا لقبول الأشخاص** **والسماح بالطلب الهاتفي المستخدمين لتجاوز الردهة** عندما يقومون بجدوله اجتماع جديد.</span><span class="sxs-lookup"><span data-stu-id="574f3-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="574f3-116">**ملاحظه:** قراءه [أداره نهج الاجتماع في الفرق](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) للحصول علي نظره عامه كامله حول نهج اجتماع فرق Microsoft.</span><span class="sxs-lookup"><span data-stu-id="574f3-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
