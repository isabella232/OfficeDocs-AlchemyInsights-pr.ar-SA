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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376501"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>ضبط إعدادات اللوبي ومستوي المشاركة

تتحكم هذه الإعدادات في الاجتماعات التي ينتظرها المشاركون في الردهة قبل قبولهم في الاجتماع ومستوي المشاركة المسموح بها في الاجتماع. يمكنك استخدام Powershell لتحديث إعدادات نهج الاجتماع التي لم يتم تنفيذها بعد (المسمي "قريبا") في مركز أداره الفرق.  انظر أدناه للحصول علي مثال cmdlet PowerShell التي تسمح لجميع المستخدمين لتجاوز الردهة.  

- [القبول التلقائي للأشخاص](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) هو نهج لكل منظم يتحكم في ما إذا كان الأشخاص ينضمون إلى الاجتماع مباشره أو ينتظرون في الردهة حتى يتم قبولهم من قبل مستخدم مصادق عليه.

- [السماح للأشخاص المجهولين ببدء اجتماع](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) هو نهج لكل منظم يتحكم في ما إذا كان بإمكان الأشخاص المجهولين ، بما في ذلك المستخدمين B2B والمتحدين ، الانضمام إلى اجتماع المستخدم بدون مستخدم مصادق عليه من المؤسسة في الحضور.

- [السماح لمستخدمي الطلب الهاتفي بتجاوز الردهة](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**قريبا**) هو نهج لكل منظم يتحكم في ما إذا كان الأشخاص الذين يقومون بالاتصال بالهاتف بالانضمام إلى الاجتماع مباشره أو الانتظار في الردهة بغض النظر عن السماح **للأشخاص** بالاعداد تلقائيا.

- [السماح للمنظمين بتجاوز إعدادات اللوبي](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**قريبا**) هو نهج لكل منظم يتحكم في ما إذا كان منظم الاجتماع يمكنه تجاوز إعدادات الردهة التي يقوم المسؤول بتعيينها **تلقائيا لقبول الأشخاص** **والسماح بالطلب الهاتفي المستخدمين لتجاوز الردهة** عندما يقومون بجدوله اجتماع جديد.

**ملاحظه:** قراءه [أداره نهج الاجتماع في الفرق](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) للحصول علي نظره عامه كامله حول نهج اجتماع فرق Microsoft. 


**مثال PowerShell**

إذا كنت ترغب في السماح للجميع ، بما في ذلك المستخدمين الخارجيين أو المجهولين ، بتجاوز اللوبي ، يمكنك أيضا استخدام PowerShell لإنجاز هذه المهمة.  في ما يلي مثال علي تعديل نهج الاجتماعات العمومية للمؤسسة الخاصة بك.   

(تاكد من مراجعه الوثائق أعلاه قبل اجراء هذه التغييرات لفهم بالبالضبط ما يسمح به هذا.)

مجموعه-كستيسميتينجينسيسينيوسيس-الهوية العالمية-أوتوادميتيدوسيرس "الجميع"-اللوبستونسسيرستوببيباسلوبي $True

للحصول علي مزيد من المعلومات ، راجع [مجموعه-كستيسميتينجيننهج](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
