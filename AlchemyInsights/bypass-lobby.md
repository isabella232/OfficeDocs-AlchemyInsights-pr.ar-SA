---
title: تجاوز ساحة الانتظار
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
- "2673"
- "9000740"
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059583"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>التحكم في إعدادات ساحة الانتظار ومستوى المشاركة في Teams

إذا كنت تريد السماح للجميع، بما في ذلك المستخدمين الذين يستخدمون الطلب الهاتفي والمستخدمين الخارجيين والمجهولين، بتجاوز ساحة الانتظار **،** فاستخدم PowerShell لتنفيذ هذه المهمة. فيما يلي مثال لتعديل نهج الاجتماع العام لمنظمتك.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

يتطلب الأمر cmdlet هذا حاليا استخدام Skype for Business PowerShell النمطية. للحصول على إعداد لاستخدام الأمر cmdlet هذا، راجع [إدارة سياسات عبر PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

بعد إعداد نهج، ستحتاج إلى تطبيقه على المستخدمين؛ أو، إذا قمت بتعديل النهج العام، سيتم تطبيقه تلقائيا على المستخدمين. لأي تغيير في النهج، يجب الانتظار 4 ساعات على الأقل حتى **24 ساعة** حتى يتم تطبيق النهج. 

تأكد من مراجعة الوثائق أدناه قبل إجراء هذه التغييرات لفهم ما يسمح به ذلك بالضبط.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>فهم Teams نهج ساحة الانتظار للاجتماعات

تتحكم هذه الإعدادات بالمشاركين في الاجتماع الذين ينتظرون في ساحة الانتظار قبل أن يسمح لهم ب المشاركة في الاجتماع ومستوى المشاركة المسموح لهم به في الاجتماع. يمكنك استخدام PowerShell لتحديث إعدادات نهج الاجتماع التي لم يتم تنفيذها بعد (المسمى "قريبا") في Teams إدارة الاجتماع. راجع أدناه للحصول على مثال PowerShell cmdlet الذي يسمح لجميع المستخدمين بتجاوز ساحة الانتظار.

- [إن قبول الأشخاص](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) تلقائيا هو نهج لكل منظم يتحكم في انضمام الأشخاص إلى اجتماع مباشرة أو الانتظار في ساحة الانتظار حتى يتم قبولهم من قبل مستخدم مصدق عليه.

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) السماح للأشخاص المجهولين ببدء اجتماع هو نهج لكل منظم يتحكم في ما إذا كان يمكن للأشخاص المجهولين، بما في ذلك B2B والمستخدمين المتصلين، الانضمام إلى اجتماع المستخدم بدون مستخدم مصدق عليه من المؤسسة الحاضرة.

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) السماح لمستخدمي الطلب بتجاوز ساحة الانتظار (قريبا)هو نهج لكل منظم يتحكم في انضمام الأشخاص الذين يتصلون هاتفيا إلى الاجتماع مباشرة أو الانتظار في ساحة الانتظار بغض النظر عن إعداد السماح للأشخاص **تلقائيا.**

- السماح للمنظمين بتجاوز إعدادات ساحة الانتظار [(قريبا)](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) هو نهج لكل منظم يتحكم في ما إذا كان يمكن لمنظم الاجتماع تجاوز  إعدادات ساحة الانتظار التي حددها المسؤول في السماح للأشخاص تلقائيا والسماح لمستخدمي الطلب بتجاوز ساحة الانتظار عند جدولة اجتماع جديد. 

**ملاحظة:** اقرأ [إدارة سياسات الاجتماعات في](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) Teams للحصول على نظرة عامة كاملة حول Microsoft Teams الاجتماعات.
