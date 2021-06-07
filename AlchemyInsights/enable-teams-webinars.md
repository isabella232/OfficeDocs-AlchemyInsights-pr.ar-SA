---
title: تمكين Teams ويب
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793518"
---
# <a name="enable-teams-webinars"></a>تمكين Teams ويب

يتم تمكين عبر الإنترنت بشكل افتراضي. يمكنك إدارة الأشخاص الذين يمكنهم جدولة الجداول Teams عبر الإنترنت باستخدام Teams PowerShell.

- يمكن أيضا لجميع المستخدمين الذين يمكنهم إنشاء اجتماع إنشاء اجتماع عبر الويب. إذا كنت تريد إدارة الأشخاص الذين يمكنهم جدولة Teams ويب، فاستخدم *AllowMeetingRegistration*. 
- بشكل افتراضي، *يتم تمكين WhoCanRegister* ثم تعيينه إلى **الجميع.** إذا كنت تريد إيقاف تشغيل تسجيل الاجتماع، فحدد *AllowMeetingRegistration إلى* **False**.

لتغيير هذه الإعدادات، يجب تثبيت Teams [PowerShell](/microsoftteams/teams-powershell-install). كما يتم فرض "سياسات الاجتماع" على Teams ويب. على سبيل المثال، إذا تم إيقاف تشغيل الانضمام المجهول في إعدادات الاجتماع، لا يمكن للمستخدمين المجهولين الانضمام إلى عبر الإنترنت.

للتعرف على المزيد حول تكوين الأشخاص الذين يمكنهم التسجيل في عبر الويب، راجع تكوين [الأشخاص الذين يمكنهم التسجيل في عبر الإنترنت](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). لمزيد من المعلومات حول إعدادات قوائم Microsoft، راجع [التحكم في إعدادات قوائم Microsoft](/sharepoint/control-lists).