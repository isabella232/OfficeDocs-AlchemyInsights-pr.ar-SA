---
title: لا يتلقى المرسل بريدا الكترونيا تم إرساله إلى مجموعه Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871578"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>لا يتلقى المرسل بريدا الكترونيا تم إرساله إلى مجموعه Microsoft 365

بشكل افتراضي ، لا يتلقى مرسل رسالة البريد الكتروني إلى مجموعه Microsoft 365 نسخه من الرسالة في علبه الوارد الخاصة به ، حتى لو كان المرسل عضوا في المجموعة.

استخدم أمر أكسو PowerShell هذا للسماح للمرسل بتلقي نسخه من كل رسالة بريد الكتروني ترسلها إلى مجموعه Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

لتمكين الاعداد لكل علب البريد في الوقت نفسه:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**ملاحظه** تستغرق التغييرات التي تم إدخالها علي هذا الاعداد إلى ساعات لتصبح ساريه المفعول.