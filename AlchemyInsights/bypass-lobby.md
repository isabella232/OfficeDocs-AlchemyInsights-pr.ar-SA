---
title: تجاوز ساحة الانتظار
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684937"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>التحكم في إعدادات الانتظار ومستوي المشاركة في الفرق

إذا أردت السماح للجميع بما في ذلك ، بما في ذلك المستخدمين الذين لديهم طلب ، وخارجي ، ومجهول ، **لتجاوز ساحة الانتظار**، فاستخدم PowerShell لإنجاز هذه المهمة. اليك مثال حول تعديل نهج الاجتماع العام لمؤسسك.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

يتطلب أمر cmdlet هذا حاليا استخدام الوحدة النمطية ل PowerShell ل business. للحصول علي اعداد لاستخدام أمر cmdlet هذا ، راجع [أداره النهج عبر PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

بمجرد اعداد نهج ، يجب تطبيقه علي المستخدمين ؛ أو ، إذا قمت بتعديل النهج العام ، سيتم تطبيقه علي المستخدمين تلقائيا. لأي تغيير في النهج ، ستحتاج إلى الانتظار لمده **4 ساعات** علي الأقل حتى 24 ساعة حتى تصبح النهج ساريه المفعول. 

تاكد من مراجعه الوثائق أدناه قبل اجراء هذه التغييرات لفهم ما يسمح به بالبالضبط.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>التعرف علي عناصر تحكم نهج ساحة انتظار اجتماعات الفرق

تتحكم هذه الإعدادات في المشاركين في الاجتماع في ساحة الانتظار قبل السماح لهم بالاجتماع ومستوي المشاركة المسموح به في اجتماع. يمكنك استخدام PowerShell لتحديث إعدادات نهج الاجتماع الذي لم يتم تطبيقه بعد (المسمي "قريبا") في مركز أداره الفرق. انظر أدناه للاطلاع علي مثال ل PowerShell cmdlet الذي يسمح لكل المستخدمين بتجاوز ساحة الانتظار.

- ان الوصول [إلى الأشخاص تلقائيا](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) هو نهج لكل منظم والذي يتحكم ما إذا كان الأشخاص ينضمون إلى اجتماع مباشره أو تنتظر في ساحة الانتظار حتى يتم السماح لهم بالإقرار بالمستخدمين المصادق عليهم.

- [السماح للأشخاص المجهولين ببدء الاجتماع](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) هو نهج لكل منظم والذي يتحكم في ما إذا كان الأشخاص المجهولين ، بما في ذلك المستخدمون من المؤسسات المتحدة الخاصة بالB2B

- [السماح لمستخدمي الطلب بتجاوز ساحة الانتظار](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) **(** قريبا) هو نهج لكل منظم الذي يتحكم بما إذا كان الأشخاص الذين يقومون بالاتصال عبر الهاتف ، انضمون إلى الاجتماع مباشره أو انتظر في ساحة الانتظار بغض النظر عن الاعداد الذي يقوم به **الأشخاص بالدخول** .

- [السماح لمنظمي بتجاوز إعدادات الانتظار](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) **(** القريبة) هو نهج لكل منظم والذي يتحكم في ما إذا كان منظم الاجتماع قد تجاوز إعدادات الانتظار التي قام المسؤول بتعيينها في العمل **تلقائيا** والسماح **لمستخدمي الطلب بتجاوز ساحة الانتظار** عند جدوله اجتماع جديد.

**ملاحظه:** أقرا [أداره نهج الاجتماع في فرق](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) للحصول علي نظره عامه حول نهج اجتماعات فرق Microsoft.
