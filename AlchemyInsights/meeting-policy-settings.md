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
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042831"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>إدارة نُهج الاجتماعات في Microsoft Teams

**ملاحظة: قد يستغرق الأمر ما يصل إلى 24 ساعة حتى تسري تغييرات النهج على المستخدمين.** قد لا تتمكن من إجراء تغييرات على النُهج التي تم إنشاؤها حديثًا على الفور؛ انتظر 4 ساعات وحاول تعديل نهج تم إنشاؤه حديثًا مرة أخرى.

يتم استخدام نُهج الاجتماع للتحكم في الميزات المتوفرة للمشاركين في الاجتماع للاجتماعات المجدولة من قبل المستخدمين في مؤسستك. قد لا يتم تنفيذ بعض ميزات نُهج الاجتماع في مركز إدارة الفرق حتى الآن (يتم تسمية هذه الميزات "قريبًا" في الوثائق). في هذه الحالة، أو إذا كنت تحصل على خطأ مثل "لا يمكننا تحديث النهج الآن ولكن حاول مرة أخرى لاحقاً" في مركز إدارة Microsoft Teams، نوصي باستخدام PowerShell لإنشاء أو تعديل نُهج اجتماع الفرق. 

لمزيد من المعلومات حول نُهج الاجتماع، راجع الموارد التالية:

- للتعرف على كيفية إنشاء النُهج وإجراء التغييرات وتعيين المستخدمين إلى النهج، راجع [إدارة نُهج الاجتماع في الفرق](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- لإجراء تغييرات في السياسة باستخدام cmdlets PowerShell، راجع [نظرة عامة على Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - تحتاج إلى استخدام [وحدة Skype for Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) لسياسات اجتماع الفرق. 
    - مراجعة [وثائق cmdlets *CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) لمزيد من المعلومات.

