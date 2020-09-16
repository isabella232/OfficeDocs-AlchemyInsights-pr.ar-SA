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
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="7eabf-102">لا يتلقى المرسل بريدا الكترونيا تم إرساله إلى مجموعه Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="7eabf-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="7eabf-103">بشكل افتراضي ، لا يتلقى مرسل رسالة البريد الكتروني إلى مجموعه Microsoft 365 نسخه من الرسالة في علبه الوارد الخاصة به ، حتى لو كان المرسل عضوا في المجموعة.</span><span class="sxs-lookup"><span data-stu-id="7eabf-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="7eabf-104">استخدم أمر أكسو PowerShell هذا للسماح للمرسل بتلقي نسخه من كل رسالة بريد الكتروني ترسلها إلى مجموعه Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="7eabf-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="7eabf-105">لتمكين الاعداد لكل علب البريد في الوقت نفسه:</span><span class="sxs-lookup"><span data-stu-id="7eabf-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="7eabf-106">**ملاحظه** تستغرق التغييرات التي تم إدخالها علي هذا الاعداد إلى ساعات لتصبح ساريه المفعول.</span><span class="sxs-lookup"><span data-stu-id="7eabf-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>