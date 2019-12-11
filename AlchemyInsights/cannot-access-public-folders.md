---
title: لا يمكن الوصول إلى المجلدات العمومية
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959482"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="8c655-102">يتعذر علي Outlook الاتصال بالمجلدات العمومية</span><span class="sxs-lookup"><span data-stu-id="8c655-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="8c655-103">إذا كان الوصول إلى المجلد العمومي لا يعمل لعدد قليل من المستخدمين ، فجرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="8c655-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="8c655-104">الاتصال ب EXO PowerShell ، وتكوين ديفاولبوبليكفولدفولبوكس علي حساب المستخدم المشكلة لمطابقه واحد علي حساب مستخدم العمل.</span><span class="sxs-lookup"><span data-stu-id="8c655-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="8c655-105">المثال:</span><span class="sxs-lookup"><span data-stu-id="8c655-105">Example:</span></span>

<span data-ttu-id="8c655-106">الحصول علي علبه البريد WorkingUser | ft ديفاولبوبليكفولدفولبوكس ، افيكتيفيبوبليكفولديرمايلبوكس</span><span class="sxs-lookup"><span data-stu-id="8c655-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="8c655-107">مجموعه-علبه البريد إشكاليه المستخدم-ديفاولبوبليكفولدفولبوكس \<من الأمر السابق></span><span class="sxs-lookup"><span data-stu-id="8c655-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="8c655-108">انتظر ساعة واحده علي الأقل حتى يسري مفعول التغيير.</span><span class="sxs-lookup"><span data-stu-id="8c655-108">Wait at least one hour for the change to take effect.</span></span>