---
title: إعدادات نهج الاجتماع
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794321"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="bc558-102">أداره نهج الاجتماع في فرق Microsoft</span><span class="sxs-lookup"><span data-stu-id="bc558-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="bc558-103">**ملاحظه: قد يستغرق الأمر مده تصل إلى 24 ساعة لكي يسري مفعول المستخدمين.**</span><span class="sxs-lookup"><span data-stu-id="bc558-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="bc558-104">قد لا تتمكن من اجراء تغييرات علي النهج التي تم إنشاؤها حديثا علي الفور ؛ انتظر 4 ساعات وحاول تعديل نهج تم إنشاؤه حديثا مره أخرى.</span><span class="sxs-lookup"><span data-stu-id="bc558-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="bc558-105">يتم استخدام نهج الاجتماع للتحكم في الميزات المتوفرة للمشاركين في الاجتماع للاجتماعات التي تمت جدولتها بواسطة المستخدمين في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="bc558-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="bc558-106">قد لا يتم تطبيق بعض ميزات نهج الاجتماع في مركز أداره الفرق حتى الآن (يتم تسميه هذه الميزات "قريبا" في الوثائق).</span><span class="sxs-lookup"><span data-stu-id="bc558-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="bc558-107">في هذه الحالة ، أو إذا كنت تتلقي رسالة خطا مثل "لا يمكننا تحديث النهج الآن ولكن جربه مره أخرى لاحقا" في مركز أداره فرق Microsoft ، نوصي باستخدام PowerShell لإنشاء سياسات اجتماعات الفرق أو تعديلها.</span><span class="sxs-lookup"><span data-stu-id="bc558-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="bc558-108">للحصول علي مزيد من المعلومات حول نهج الاجتماع ، راجع الموارد التالية:</span><span class="sxs-lookup"><span data-stu-id="bc558-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="bc558-109">للتعرف علي كيفيه إنشاء النهج واجراء التغييرات وتعيين المستخدمين إلى النهج ، راجع [أداره نهج الاجتماع في الفرق](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="bc558-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="bc558-110">لاجراء تغييرات علي النهج باستخدام أوامر PowerShell cmdlets ، راجع [نظره عامه حول الفرق في powershell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="bc558-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="bc558-111">أنت بحاجه إلى استخدام [الوحدة النمطية ل PowerShell ل Skype For business](https://www.microsoft.com/download/details.aspx?id=39366) لنهج اجتماعات الفرق.</span><span class="sxs-lookup"><span data-stu-id="bc558-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="bc558-112">راجع [وثائق cmdlets لكستيمسميتينجبوليسي](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="bc558-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

