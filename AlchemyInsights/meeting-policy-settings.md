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
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627561"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="a8ebb-102">أداره نهج الاجتماعات في فرق Microsoft</span><span class="sxs-lookup"><span data-stu-id="a8ebb-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="a8ebb-103">يتم استخدام نهج الاجتماعات للتحكم في الميزات المتوفرة للمشاركين في الاجتماعات للاجتماعات المجدولة من قبل المستخدمين في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="a8ebb-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="a8ebb-104">قد لا يتم تنفيذ بعض ميزات نهج الاجتماع في مركز أداره الفرق بعد (تسمي هذه "قريبا" في الوثائق).</span><span class="sxs-lookup"><span data-stu-id="a8ebb-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="a8ebb-105">في هذه الحالة ، أو إذا كنت تحصل علي خطا مثل "لا يمكننا تحديث النهج في الوقت الحالي ولكن حاول مره أخرى لاحقا" في مركز أداره الفرق Microsoft ، نوصي باستخدام PowerShell لإنشاء أو تعديل نهج اجتماع الفرق.</span><span class="sxs-lookup"><span data-stu-id="a8ebb-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="a8ebb-106">لمزيد من المعلومات حول نهج الاجتماع ، راجع الموارد التالية:</span><span class="sxs-lookup"><span data-stu-id="a8ebb-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="a8ebb-107">للتعرف علي كيفيه إنشاء النهج واجراء التغييرات وتعيين المستخدمين إلى النهج ، راجع [أداره نهج الاجتماعات في الفرق](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="a8ebb-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="a8ebb-108">لاجراء تغييرات في النهج باستخدام cmdlets PowerShell ، راجع [نظره عامه حول powershell الفرق](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="a8ebb-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="a8ebb-109">تحتاج إلى استخدام [سكايب الوحدة النمطية PowerShell الاعمال](https://www.microsoft.com/download/details.aspx?id=39366) لنهج الاجتماع فرق.</span><span class="sxs-lookup"><span data-stu-id="a8ebb-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="a8ebb-110">مراجعه [وثائق cmdlets \*-كستيسميتينجينجسيسينينسيس](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="a8ebb-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="a8ebb-111">**ملاحظه:** يمكن ان يستغرق ما يصل إلى 24 ساعة لتغييرات السياسة نافذه المفعول بالنسبة للمستخدمين.</span><span class="sxs-lookup"><span data-stu-id="a8ebb-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="a8ebb-112">قد لا تتمكن من اجراء تغييرات علي النهج التي تم إنشاؤها حديثا علي الفور; الانتظار 4 ساعات ومحاولة تعديل نهج تم إنشاؤه حديثا مره أخرى.</span><span class="sxs-lookup"><span data-stu-id="a8ebb-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="a8ebb-113">إذا كنت لا تزال تواجه مشاكل ، فجرب PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a8ebb-113">If you're still having problems, try PowerShell.</span></span>  