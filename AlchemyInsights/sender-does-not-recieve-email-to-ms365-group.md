---
title: لا يتلقى المرسل بريدا الكترونيا تم إرساله إلى مجموعه Microsoft 365
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
ms.openlocfilehash: b8091305d55408f51cf369506acc7bfac59defb5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751302"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>لا يتلقى المرسل بريدا الكترونيا تم إرساله إلى مجموعه Microsoft 365

بشكل افتراضي ، لا يتلقى مرسل رسالة البريد الكتروني إلى مجموعه Microsoft 365 نسخه من الرسالة في علبه الوارد الخاصة به ، حتى لو كان المرسل عضوا في المجموعة.

استخدم أمر أكسو PowerShell هذا للسماح للمرسل بتلقي نسخه من كل رسالة بريد الكتروني ترسلها إلى مجموعه Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

لتمكين الاعداد لكل علب البريد في الوقت نفسه:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**ملاحظه** تستغرق التغييرات التي تم إدخالها علي هذا الاعداد إلى ساعات لتصبح ساريه المفعول.