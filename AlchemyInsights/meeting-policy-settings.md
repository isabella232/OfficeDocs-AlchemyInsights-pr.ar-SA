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
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794321"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>أداره نهج الاجتماع في فرق Microsoft

**ملاحظه: قد يستغرق الأمر مده تصل إلى 24 ساعة لكي يسري مفعول المستخدمين.** قد لا تتمكن من اجراء تغييرات علي النهج التي تم إنشاؤها حديثا علي الفور ؛ انتظر 4 ساعات وحاول تعديل نهج تم إنشاؤه حديثا مره أخرى.

يتم استخدام نهج الاجتماع للتحكم في الميزات المتوفرة للمشاركين في الاجتماع للاجتماعات التي تمت جدولتها بواسطة المستخدمين في مؤسستك. قد لا يتم تطبيق بعض ميزات نهج الاجتماع في مركز أداره الفرق حتى الآن (يتم تسميه هذه الميزات "قريبا" في الوثائق). في هذه الحالة ، أو إذا كنت تتلقي رسالة خطا مثل "لا يمكننا تحديث النهج الآن ولكن جربه مره أخرى لاحقا" في مركز أداره فرق Microsoft ، نوصي باستخدام PowerShell لإنشاء سياسات اجتماعات الفرق أو تعديلها. 

للحصول علي مزيد من المعلومات حول نهج الاجتماع ، راجع الموارد التالية:

- للتعرف علي كيفيه إنشاء النهج واجراء التغييرات وتعيين المستخدمين إلى النهج ، راجع [أداره نهج الاجتماع في الفرق](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- لاجراء تغييرات علي النهج باستخدام أوامر PowerShell cmdlets ، راجع [نظره عامه حول الفرق في powershell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - أنت بحاجه إلى استخدام [الوحدة النمطية ل PowerShell ل Skype For business](https://www.microsoft.com/download/details.aspx?id=39366) لنهج اجتماعات الفرق. 
    - راجع [وثائق cmdlets لكستيمسميتينجبوليسي](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) للحصول علي مزيد من المعلومات.

