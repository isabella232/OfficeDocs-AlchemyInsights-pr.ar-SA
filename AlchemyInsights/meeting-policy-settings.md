---
title: إعدادات نهج الاجتماع
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925152"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>إدارة سياسات الاجتماعات في Microsoft Teams

**ملاحظة: قد يستغرق الأمر ما يصل إلى 24 ساعة حتى يتم وضع تغييرات النهج حيز التنفيذ للمستخدمين.** قد لا تتمكن من إجراء تغييرات على السياسات التي تم إنشاؤها حديثا على الفور؛ انتظر 4 ساعات ثم حاول تعديل نهج تم إنشاؤه حديثا مرة أخرى.

يتم استخدام سياسات الاجتماع للتحكم في الميزات المتوفرة للمشاركين في الاجتماع للاجتماعات المجدولة بواسطة المستخدمين في مؤسستك. قد لا يتم تنفيذ بعض ميزات سياسات الاجتماعات في مركز إدارة Teams بعد (تسمى هذه الميزات "قريبا" في الوثائق). في هذه الحالة، أو إذا كنت تحصل على خطأ مثل "لا يمكننا تحديث النهج الآن ولكن حاول مرة أخرى لاحقا" في مركز إدارة Microsoft Teams، فإننا نوصي باستخدام PowerShell لإنشاء نهج اجتماعات Teams أو تعديلها. 

لمزيد من المعلومات حول سياسات الاجتماعات، راجع الموارد التالية:

- للتعرف على كيفية إنشاء النهج، وأية تغييرات، وتعيين مستخدمين إلى النهج، راجع إدارة نهج الاجتماعات [في Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- بإجراء تغييرات على النهج باستخدام PowerShell cmdlets، راجع Teams [نظرة عامة حول PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - تحتاج إلى استخدام الوحدة النمطية Skype for Business [PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) Teams الاجتماعات. 
    - راجع [وثائق cmdlets *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) للحصول على مزيد من المعلومات.

