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
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376496"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>أداره نهج الاجتماعات في فرق Microsoft

يتم استخدام نهج الاجتماعات للتحكم في الميزات المتوفرة للمشاركين في الاجتماعات للاجتماعات المجدولة من قبل المستخدمين في مؤسستك. قد لا يتم تنفيذ بعض ميزات نهج الاجتماع في مركز أداره الفرق بعد (تسمي هذه "قريبا" في الوثائق). في هذه الحالة ، أو إذا كنت تحصل علي خطا مثل "لا يمكننا تحديث النهج في الوقت الحالي ولكن حاول مره أخرى لاحقا" في مركز أداره الفرق Microsoft ، نوصي باستخدام PowerShell لإنشاء أو تعديل نهج اجتماع الفرق. 

لمزيد من المعلومات حول نهج الاجتماع ، راجع الموارد التالية:

- للتعرف علي كيفيه إنشاء النهج واجراء التغييرات وتعيين المستخدمين إلى النهج ، راجع [أداره نهج الاجتماعات في الفرق](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).

- لاجراء تغييرات في النهج باستخدام cmdlets PowerShell ، راجع [نظره عامه حول powershell الفرق](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - تحتاج إلى استخدام [سكايب الوحدة النمطية PowerShell الاعمال](https://www.microsoft.com/download/details.aspx?id=39366) لنهج الاجتماع فرق. 
    - مراجعه [وثائق cmdlets *-كستيسميتينجينجسيسينينسيس](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) للحصول علي مزيد من المعلومات.

**ملاحظه:** يمكن ان يستغرق ما يصل إلى 24 ساعة لتغييرات السياسة نافذه المفعول بالنسبة للمستخدمين. قد لا تتمكن من اجراء تغييرات علي النهج التي تم إنشاؤها حديثا علي الفور; الانتظار 4 ساعات ومحاولة تعديل نهج تم إنشاؤه حديثا مره أخرى. إذا كنت لا تزال تواجه مشاكل ، فجرب PowerShell.  