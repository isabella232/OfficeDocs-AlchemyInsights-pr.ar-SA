---
title: إدارة تسجيل ندوة عبر الويب
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793534"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="7c561-102">إدارة تسجيل ندوة عبر الويب</span><span class="sxs-lookup"><span data-stu-id="7c561-102">Manage webinar registration</span></span>

<span data-ttu-id="7c561-103">يمكنك إدارة الأشخاص الذين يمكنهم التسجيل للحصول على Teams ويب باستخدام Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="7c561-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="7c561-104">لتثبيت Powershell Teams، راجع Teams [PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="7c561-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="7c561-105">بشكل افتراضي، *يتم تمكين WhoCanRegister* ثم تعيينها إلى **EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="7c561-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="7c561-106">للسماح لأي شخص، بما في ذلك المستخدمين المجهولين، بالتسجيل، يجب تعيين نهج الاجتماع للجميع باستخدام الأمر Powershell: </span><span class="sxs-lookup"><span data-stu-id="7c561-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="7c561-107">**ملاحظة:** إذا تم إيقاف تشغيل الانضمام المجهول في إعدادات الاجتماع، لا يمكن للمستخدمين المجهولين الانضمام إلى عقد عبر الويب.</span><span class="sxs-lookup"><span data-stu-id="7c561-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="7c561-108">لمعرفة المزيد وتمكين هذا الإعداد، راجع إدارة إعدادات [الاجتماع في Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="7c561-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="7c561-109">إذا كنت تريد إيقاف تشغيل تسجيل الاجتماع، فحدد *AllowMeetingRegistration إلى* **False**.</span><span class="sxs-lookup"><span data-stu-id="7c561-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="7c561-110">للتعرف على المزيد حول تكوين الأشخاص الذين يمكنهم التسجيل في عبر الويب، راجع تكوين [الأشخاص الذين يمكنهم التسجيل في عبر الإنترنت](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="7c561-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="7c561-111">لمزيد من المعلومات حول إعدادات قوائم Microsoft، راجع [التحكم في إعدادات قوائم Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="7c561-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
