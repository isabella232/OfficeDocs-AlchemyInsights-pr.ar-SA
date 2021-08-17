---
title: كيفية تمكين البريد الصوتي المستضاف
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055541"
---
# <a name="how-to-enable-hosted-voicemail"></a>كيفية تمكين البريد الصوتي المستضاف

لتمكين البريد الصوتي، يجب تعيين **HostedVoicemail** إلى $true.

الخاصية **HostedVoicemail** على المستخدم باستخدام Remote PowerShell (RPS).

لمزيد من المعلومات حول الاتصال ب RPS، راجع Microsoft Teams نظرة عامة حول [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) للحصول على مزيد من المعلومات حول الاتصال ب RPS.

1. يجب Teams تسجيل الدخول إلى Remote PowerShell Teams.
1. من PowerShell، Teams يمكن للمسؤول تشغيل **set-csuser user@contoso.com -HostedVoiceMail $true** حيث يكون sip uri من المستخدم المعني.

> [!NOTE]
> قد تستغرق التغييرات التي يتم إدخالها على السياسات ما يصل إلى 24 ساعة للتكرار.