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
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704593"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="2edd7-102">إدارة سياسات الاجتماعات في Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2edd7-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="2edd7-103">**ملاحظة: قد يستغرق الأمر ما يصل إلى 24 ساعة حتى يتم تأثير تغييرات النهج للمستخدمين.**</span><span class="sxs-lookup"><span data-stu-id="2edd7-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="2edd7-104">قد لا تتمكن من إجراء تغييرات على السياسات التي تم إنشاؤها حديثا على الفور؛ انتظر 4 ساعات ثم حاول تعديل نهج تم إنشاؤه حديثا مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="2edd7-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="2edd7-105">تستخدم سياسات الاجتماعات للتحكم في الميزات المتوفرة للمشاركين في الاجتماع للاجتماعات المجدولة بواسطة المستخدمين في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="2edd7-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="2edd7-106">قد لا يتم تنفيذ بعض ميزات سياسات الاجتماعات في مركز إدارة Teams بعد (تسمى هذه الميزات "قريبا" في الوثائق).</span><span class="sxs-lookup"><span data-stu-id="2edd7-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="2edd7-107">في هذه الحالة، أو إذا كنت تحصل على خطأ مثل "لا يمكننا تحديث النهج الآن ولكن حاول مرة أخرى لاحقا" في مركز إدارة Microsoft Teams، نوصي باستخدام PowerShell لإنشاء نهج اجتماعات Teams أو تعديلها.</span><span class="sxs-lookup"><span data-stu-id="2edd7-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="2edd7-108">لمزيد من المعلومات حول سياسات الاجتماع، راجع الموارد التالية:</span><span class="sxs-lookup"><span data-stu-id="2edd7-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="2edd7-109">للتعرف على كيفية إنشاء النهج، وأية تغييرات، وتعيين مستخدمين إلى النهج، راجع إدارة نهج [الاجتماعات في Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="2edd7-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="2edd7-110">بإجراء تغييرات على النهج باستخدام PowerShell cmdlets، راجع [نظرة عامة على Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="2edd7-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="2edd7-111">أنت بحاجة إلى استخدام وحدة [Skype for Business PowerShell النمطية](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) لنهج اجتماعات Teams.</span><span class="sxs-lookup"><span data-stu-id="2edd7-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="2edd7-112">راجع [وثائق cmdlets \*-CsTeamsMeetingPolicy cmdlets](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="2edd7-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

