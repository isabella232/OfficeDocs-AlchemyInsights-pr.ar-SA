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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376501"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="8e137-102">ضبط إعدادات اللوبي ومستوي المشاركة</span><span class="sxs-lookup"><span data-stu-id="8e137-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="8e137-103">تتحكم هذه الإعدادات في الاجتماعات التي ينتظرها المشاركون في الردهة قبل قبولهم في الاجتماع ومستوي المشاركة المسموح بها في الاجتماع.</span><span class="sxs-lookup"><span data-stu-id="8e137-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="8e137-104">يمكنك استخدام Powershell لتحديث إعدادات نهج الاجتماع التي لم يتم تنفيذها بعد (المسمي "قريبا") في مركز أداره الفرق.</span><span class="sxs-lookup"><span data-stu-id="8e137-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="8e137-105">انظر أدناه للحصول علي مثال cmdlet PowerShell التي تسمح لجميع المستخدمين لتجاوز الردهة.</span><span class="sxs-lookup"><span data-stu-id="8e137-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="8e137-106">[القبول التلقائي للأشخاص](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) هو نهج لكل منظم يتحكم في ما إذا كان الأشخاص ينضمون إلى الاجتماع مباشره أو ينتظرون في الردهة حتى يتم قبولهم من قبل مستخدم مصادق عليه.</span><span class="sxs-lookup"><span data-stu-id="8e137-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="8e137-107">[السماح للأشخاص المجهولين ببدء اجتماع](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) هو نهج لكل منظم يتحكم في ما إذا كان بإمكان الأشخاص المجهولين ، بما في ذلك المستخدمين B2B والمتحدين ، الانضمام إلى اجتماع المستخدم بدون مستخدم مصادق عليه من المؤسسة في الحضور.</span><span class="sxs-lookup"><span data-stu-id="8e137-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="8e137-108">[السماح لمستخدمي الطلب الهاتفي بتجاوز الردهة](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**قريبا**) هو نهج لكل منظم يتحكم في ما إذا كان الأشخاص الذين يقومون بالاتصال بالهاتف بالانضمام إلى الاجتماع مباشره أو الانتظار في الردهة بغض النظر عن السماح **للأشخاص** بالاعداد تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="8e137-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="8e137-109">[السماح للمنظمين بتجاوز إعدادات اللوبي](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**قريبا**) هو نهج لكل منظم يتحكم في ما إذا كان منظم الاجتماع يمكنه تجاوز إعدادات الردهة التي يقوم المسؤول بتعيينها **تلقائيا لقبول الأشخاص** **والسماح بالطلب الهاتفي المستخدمين لتجاوز الردهة** عندما يقومون بجدوله اجتماع جديد.</span><span class="sxs-lookup"><span data-stu-id="8e137-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="8e137-110">**ملاحظه:** قراءه [أداره نهج الاجتماع في الفرق](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) للحصول علي نظره عامه كامله حول نهج اجتماع فرق Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8e137-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="8e137-111">**مثال PowerShell**</span><span class="sxs-lookup"><span data-stu-id="8e137-111">**PowerShell example**</span></span>

<span data-ttu-id="8e137-112">إذا كنت ترغب في السماح للجميع ، بما في ذلك المستخدمين الخارجيين أو المجهولين ، بتجاوز اللوبي ، يمكنك أيضا استخدام PowerShell لإنجاز هذه المهمة.</span><span class="sxs-lookup"><span data-stu-id="8e137-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="8e137-113">في ما يلي مثال علي تعديل نهج الاجتماعات العمومية للمؤسسة الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="8e137-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="8e137-114">(تاكد من مراجعه الوثائق أعلاه قبل اجراء هذه التغييرات لفهم بالبالضبط ما يسمح به هذا.)</span><span class="sxs-lookup"><span data-stu-id="8e137-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="8e137-115">مجموعه-كستيسميتينجينسيسينيوسيس-الهوية العالمية-أوتوادميتيدوسيرس "الجميع"-اللوبستونسسيرستوببيباسلوبي $True</span><span class="sxs-lookup"><span data-stu-id="8e137-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="8e137-116">للحصول علي مزيد من المعلومات ، راجع [مجموعه-كستيسميتينجيننهج](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="8e137-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
