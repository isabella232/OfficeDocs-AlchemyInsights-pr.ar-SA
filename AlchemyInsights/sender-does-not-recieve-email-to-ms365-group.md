---
title: لا يتلقى المرسل بريدا إلكترونيا مرسلا إلى Microsoft 365 المجموعة
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 893b80567567590357a638370b8c8d58b87a98a51c68cfcc84629eda5ac71b44
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958284"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>لا يتلقى المرسل بريدا إلكترونيا مرسلا إلى Microsoft 365 المجموعة

بشكل افتراضي، لا يتلقى مرسل رسالة بريد إلكتروني إلى مجموعة Microsoft 365 نسخة من الرسالة في علبة الوارد الخاصة به، حتى لو كان المرسل عضوا في المجموعة.

استخدم أمر EXO PowerShell هذا للسماح للمرسل بتلقي نسخة من كل رسالة بريد إلكتروني يرسلها إلى مجموعة Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

لتمكين الإعداد لكل علب البريد مرة واحدة:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**ملاحظة** تستغرق التغييرات التي يتم إدخالها على هذا الإعداد ما يصل إلى ساعة لكي يتم تطبيقها.