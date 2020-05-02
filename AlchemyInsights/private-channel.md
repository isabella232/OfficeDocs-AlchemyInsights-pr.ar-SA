---
title: قناة خاصة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005425"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="cb021-102">القنوات الخاصة في فرق Microsoft</span><span class="sxs-lookup"><span data-stu-id="cb021-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="cb021-103">القنوات الخاصة هي ميزة جديدة في Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="cb021-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="cb021-104">لاحظ أنه لا يمكن تحويل القنوات الخاصة من القنوات القياسية أو العكس بالعكس.</span><span class="sxs-lookup"><span data-stu-id="cb021-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="cb021-105">للحصول على تفاصيل حول القنوات الخاصة، مثل معلومات حول [إنشاء القنوات الخاصة والعضوية](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) [ومواقع SharePoint الخاصة،](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)راجع [القنوات الخاصة في Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="cb021-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="cb021-106">**ملاحظة:** نظرًا لأن التكوين للاحتفاظ برسائل القناة الخاصة غير معتمد بعد، فلن يكون لدى المستأجرين الذين لديهم نُهج الاحتفاظ ممكّنة قنوات خاصة ممكّنة بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="cb021-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="cb021-107">يمكن تمكين القنوات الخاصة في مركز إدارة Teams.</span><span class="sxs-lookup"><span data-stu-id="cb021-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="cb021-108">أيضاً، لاحظ أنه في حين أن الاحتفاظ برسائل القناة الخاصة غير معتمد، يتم دعم الاحتفاظ بالملفات المشتركة في القنوات الخاصة.</span><span class="sxs-lookup"><span data-stu-id="cb021-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="cb021-109">**هل تحتاج إلى مالك فريق جديد؟**</span><span class="sxs-lookup"><span data-stu-id="cb021-109">**Need a new team owner?**</span></span>

<span data-ttu-id="cb021-110">إذا غادر مالك قناتك الخاصة، يمكنك إضافة مالك فريق جديد عبر Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="cb021-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="cb021-111">انتقل إلى [هنا](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) لتثبيت فرق Powershell.</span><span class="sxs-lookup"><span data-stu-id="cb021-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="cb021-112">هنا هو cmdlet سوف تحتاج:</span><span class="sxs-lookup"><span data-stu-id="cb021-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="cb021-113">لمزيد من المعلومات حول فرق Powershell، راجع [نظرة عامة على Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="cb021-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
