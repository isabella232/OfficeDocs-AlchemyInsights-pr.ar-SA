---
title: الردهة التفافيه
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 6632bb0c09c7ce99f14cd55582025b37a846369d
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/25/2019
ms.locfileid: "37654243"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>ضبط إعدادات اللوبي ومستوي المشاركة

إذا كنت ترغب في السماح للجميع ، بما في ذلك المستخدمين الهاتفيين والخارجيين والمجهولين بتجاوز اللوبي ، يمكنك استخدام PowerShell للقيام بذلك. في ما يلي مثال علي تعديل نهج الاجتماعات العمومية للمؤسسة الخاصة بك:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

يتطلب هذا cmdlet حاليا استخدام سكايب للوحدة النمطية PowerShell الاعمال. للحصول علي الاعداد لاستخدام هذا cmdlet ، تحقق من [أداره النهج عبر PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

يمكنك اعداد سياسة جديده ، والتي ستحتاج بعد ذلك إلى تطبيقها علي المستخدمين. إذا قمت بتعديل النهج العمومي سيتم تطبيقه تلقائيا علي المستخدمين. لأي تغيير في السياسة تحتاج إلى الانتظار 4 ساعات علي الأقل وتصل إلى 24 ساعة حتى تسري السياسات.

تاكد من مراجعه الوثائق أدناه قبل اجراء هذه التغييرات لفهم ما يسمح به هذا بالبالضبط.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>فهم فرق التحكم في نهج اللوبي

- [القبول التلقائي للأشخاص](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) هو نهج لكل منظم يتحكم في ما إذا كان الأشخاص ينضمون إلى الاجتماع مباشره أو ينتظرون في الردهة حتى يتم قبولهم من قبل مستخدم مصادق عليه.

- [السماح للأشخاص المجهولين ببدء اجتماع](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) هو نهج لكل منظم يتحكم في ما إذا كان بإمكان الأشخاص المجهولين ، بما في ذلك المستخدمين B2B والمتحدين ، الانضمام إلى اجتماع المستخدم بدون مستخدم مصادق عليه من المؤسسة في الحضور.

- [السماح لمستخدمي الطلب الهاتفي بتجاوز الردهة](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**قريبا**) هو نهج لكل منظم يتحكم في ما إذا كان الأشخاص الذين يقومون بالاتصال بالهاتف بالانضمام إلى الاجتماع مباشره أو الانتظار في الردهة بغض النظر عن السماح **للأشخاص** بالاعداد تلقائيا.

- [السماح للمنظمين بتجاوز إعدادات اللوبي](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**قريبا**) هو نهج لكل منظم يتحكم في ما إذا كان منظم الاجتماع يمكنه تجاوز إعدادات الردهة التي يقوم المسؤول بتعيينها **تلقائيا لقبول الأشخاص** **والسماح بالطلب الهاتفي المستخدمين لتجاوز الردهة** عندما يقومون بجدوله اجتماع جديد.

**ملاحظه:** قراءه [أداره نهج الاجتماع في الفرق](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) للحصول علي نظره عامه كامله حول نهج اجتماع فرق Microsoft.
