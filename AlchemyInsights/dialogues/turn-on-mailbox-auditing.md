---
title: تشغيل تدقيق علبة البريد
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429225"
---
# <a name="turn-on-mailbox-auditing"></a>تشغيل تدقيق علبة البريد

لتشغيل تدقيق علبة البريد لمستخدم واحد أو مؤسسة بأكملها، قم بتشغيل cmdlets التالية من Remote PowerShell:

- **مستخدم واحد**: Set-Mailbox Identity "Jane Dow" -AuditEnabled $true
- **المؤسسة**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

لمعرفة المزيد، راجع ["إدارة تدقيق علبة البريد".](https://go.microsoft.com/fwlink/?linkid=2103668)