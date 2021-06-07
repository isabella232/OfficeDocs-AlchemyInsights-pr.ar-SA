---
title: تمكين Teams ويب
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793518"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="a17b3-102">تمكين Teams ويب</span><span class="sxs-lookup"><span data-stu-id="a17b3-102">Enable Teams Webinars</span></span>

<span data-ttu-id="a17b3-103">يتم تمكين عبر الإنترنت بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="a17b3-103">Webinars are enabled by default.</span></span> <span data-ttu-id="a17b3-104">يمكنك إدارة الأشخاص الذين يمكنهم جدولة الجداول Teams عبر الإنترنت باستخدام Teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a17b3-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="a17b3-105">يمكن أيضا لجميع المستخدمين الذين يمكنهم إنشاء اجتماع إنشاء اجتماع عبر الويب.</span><span class="sxs-lookup"><span data-stu-id="a17b3-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="a17b3-106">إذا كنت تريد إدارة الأشخاص الذين يمكنهم جدولة Teams ويب، فاستخدم *AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="a17b3-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="a17b3-107">بشكل افتراضي، *يتم تمكين WhoCanRegister* ثم تعيينه إلى **الجميع.**</span><span class="sxs-lookup"><span data-stu-id="a17b3-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="a17b3-108">إذا كنت تريد إيقاف تشغيل تسجيل الاجتماع، فحدد *AllowMeetingRegistration إلى* **False**.</span><span class="sxs-lookup"><span data-stu-id="a17b3-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="a17b3-109">لتغيير هذه الإعدادات، يجب تثبيت Teams [PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="a17b3-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="a17b3-110">كما يتم فرض "سياسات الاجتماع" على Teams ويب.</span><span class="sxs-lookup"><span data-stu-id="a17b3-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="a17b3-111">على سبيل المثال، إذا تم إيقاف تشغيل الانضمام المجهول في إعدادات الاجتماع، لا يمكن للمستخدمين المجهولين الانضمام إلى عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="a17b3-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="a17b3-112">للتعرف على المزيد حول تكوين الأشخاص الذين يمكنهم التسجيل في عبر الويب، راجع تكوين [الأشخاص الذين يمكنهم التسجيل في عبر الإنترنت](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="a17b3-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="a17b3-113">لمزيد من المعلومات حول إعدادات قوائم Microsoft، راجع [التحكم في إعدادات قوائم Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="a17b3-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>