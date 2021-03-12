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
# <a name="manage-meeting-policies-in-microsoft-teams"></a>إدارة سياسات الاجتماعات في Microsoft Teams

**ملاحظة: قد يستغرق الأمر ما يصل إلى 24 ساعة حتى يتم تأثير تغييرات النهج للمستخدمين.** قد لا تتمكن من إجراء تغييرات على السياسات التي تم إنشاؤها حديثا على الفور؛ انتظر 4 ساعات ثم حاول تعديل نهج تم إنشاؤه حديثا مرة أخرى.

تستخدم سياسات الاجتماعات للتحكم في الميزات المتوفرة للمشاركين في الاجتماع للاجتماعات المجدولة بواسطة المستخدمين في مؤسستك. قد لا يتم تنفيذ بعض ميزات سياسات الاجتماعات في مركز إدارة Teams بعد (تسمى هذه الميزات "قريبا" في الوثائق). في هذه الحالة، أو إذا كنت تحصل على خطأ مثل "لا يمكننا تحديث النهج الآن ولكن حاول مرة أخرى لاحقا" في مركز إدارة Microsoft Teams، نوصي باستخدام PowerShell لإنشاء نهج اجتماعات Teams أو تعديلها. 

لمزيد من المعلومات حول سياسات الاجتماع، راجع الموارد التالية:

- للتعرف على كيفية إنشاء النهج، وأية تغييرات، وتعيين مستخدمين إلى النهج، راجع إدارة نهج [الاجتماعات في Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- بإجراء تغييرات على النهج باستخدام PowerShell cmdlets، راجع [نظرة عامة على Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - أنت بحاجة إلى استخدام وحدة [Skype for Business PowerShell النمطية](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) لنهج اجتماعات Teams. 
    - راجع [وثائق cmdlets *-CsTeamsMeetingPolicy cmdlets](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) للحصول على مزيد من المعلومات.

