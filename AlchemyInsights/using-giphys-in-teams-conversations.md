---
title: استخدام Giphys في محادثات الفرق
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982419"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="0db9d-102">استخدام Giphys في محادثات الفرق</span><span class="sxs-lookup"><span data-stu-id="0db9d-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="0db9d-103">يتم تمكين الوصول إلى Giphys في دردشة الفرق بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="0db9d-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="0db9d-104">بصفتك المسؤول ، يمكنك التحكم في ما إذا كانت Giphys متوفرة للمستخدمين من خلال [تعيين نهج المراسلة](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) والتاكد من ان **استخدام Giphys في المحادثات** قيد **التشغيل**.</span><span class="sxs-lookup"><span data-stu-id="0db9d-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="0db9d-105">إذا لم تعمل صور Gif كما هو متوقع في محادثات الفرق ، فتحقق من:</span><span class="sxs-lookup"><span data-stu-id="0db9d-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="0db9d-106">يحتاج [نهج المراسلة](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) إلى السماح بالGiphys.</span><span class="sxs-lookup"><span data-stu-id="0db9d-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="0db9d-107">للتحقق من الصحة باستخدام أوامر PowerShell cmdlets:</span><span class="sxs-lookup"><span data-stu-id="0db9d-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="0db9d-108">تاكد من انه يمكنك [أداره الفرق باستخدام PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="0db9d-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="0db9d-109">قم بتشغيل [الكستيمسميساجينجبوليسي العام](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) الخاص بالأمر PowerShell والتحقق من تعيين **اللووجيفي** إلى **TRUE**.</span><span class="sxs-lookup"><span data-stu-id="0db9d-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="0db9d-110">إذا تم تعيين **اللووجيفي** إلى **FALSE** ، فقم بتشغيل مجموعه أوامر PowerShell [التالية-ال$True اللووجيفي العامة](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)الخاصة بالكستيمسميساجينجبوليسي.</span><span class="sxs-lookup"><span data-stu-id="0db9d-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="0db9d-111">يجب تمكين [التجربة المتصلة الاختيارية](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) للسماح بالوصول إلى عنوان URL لجيفي.</span><span class="sxs-lookup"><span data-stu-id="0db9d-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="0db9d-112">إذا كان لديك العديد من النهج الخاصة بالمراسلة التي تم تكوينها للمستاجر المستاجر ، فيمكنك تحديد هويه النهج المعين إلى المستخدم المتاثر باستخدام الأمر PowerShell [كسونلينيوسير الحصول علي الهوية](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | حدد تيمسميساجينجبوليسي.</span><span class="sxs-lookup"><span data-stu-id="0db9d-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
