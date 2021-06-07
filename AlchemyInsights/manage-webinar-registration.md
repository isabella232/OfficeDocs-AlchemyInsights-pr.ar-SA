---
title: إدارة تسجيل ندوة عبر الويب
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793534"
---
# <a name="manage-webinar-registration"></a>إدارة تسجيل ندوة عبر الويب

يمكنك إدارة الأشخاص الذين يمكنهم التسجيل للحصول على Teams ويب باستخدام Teams Powershell. لتثبيت Powershell Teams، راجع Teams [PowerShell](/microsoftteams/teams-powershell-install). 

بشكل افتراضي، *يتم تمكين WhoCanRegister* ثم تعيينها إلى **EveryoneInCompany**. للسماح لأي شخص، بما في ذلك المستخدمين المجهولين، بالتسجيل، يجب تعيين نهج الاجتماع للجميع باستخدام الأمر Powershell: 

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**ملاحظة:** إذا تم إيقاف تشغيل الانضمام المجهول في إعدادات الاجتماع، لا يمكن للمستخدمين المجهولين الانضمام إلى عقد عبر الويب. لمعرفة المزيد وتمكين هذا الإعداد، راجع إدارة إعدادات [الاجتماع في Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

إذا كنت تريد إيقاف تشغيل تسجيل الاجتماع، فحدد *AllowMeetingRegistration إلى* **False**.

للتعرف على المزيد حول تكوين الأشخاص الذين يمكنهم التسجيل في عبر الويب، راجع تكوين [الأشخاص الذين يمكنهم التسجيل في عبر الإنترنت](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). لمزيد من المعلومات حول إعدادات قوائم Microsoft، راجع [التحكم في إعدادات قوائم Microsoft](/sharepoint/control-lists).
