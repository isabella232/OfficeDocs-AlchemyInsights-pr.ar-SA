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
# <a name="private-channels-in-microsoft-teams"></a>القنوات الخاصة في فرق Microsoft

القنوات الخاصة هي ميزة جديدة في Microsoft Teams. لاحظ أنه لا يمكن تحويل القنوات الخاصة من القنوات القياسية أو العكس بالعكس.

للحصول على تفاصيل حول القنوات الخاصة، مثل معلومات حول [إنشاء القنوات الخاصة والعضوية](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) [ومواقع SharePoint الخاصة،](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)راجع [القنوات الخاصة في Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**ملاحظة:** نظرًا لأن التكوين للاحتفاظ برسائل القناة الخاصة غير معتمد بعد، فلن يكون لدى المستأجرين الذين لديهم نُهج الاحتفاظ ممكّنة قنوات خاصة ممكّنة بشكل افتراضي. يمكن تمكين القنوات الخاصة في مركز إدارة Teams. أيضاً، لاحظ أنه في حين أن الاحتفاظ برسائل القناة الخاصة غير معتمد، يتم دعم الاحتفاظ بالملفات المشتركة في القنوات الخاصة.

**هل تحتاج إلى مالك فريق جديد؟**

إذا غادر مالك قناتك الخاصة، يمكنك إضافة مالك فريق جديد عبر Teams Powershell.


- انتقل إلى [هنا](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) لتثبيت فرق Powershell.

هنا هو cmdlet سوف تحتاج:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

لمزيد من المعلومات حول فرق Powershell، راجع [نظرة عامة على Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
