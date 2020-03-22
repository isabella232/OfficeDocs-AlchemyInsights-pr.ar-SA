---
title: لا يمكن الوصول إلى المجلدات العامة
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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891736"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="b4052-102">لا يمكن لـ Outlook الاتصال بالمجلدات العامة</span><span class="sxs-lookup"><span data-stu-id="b4052-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="b4052-103">إذا كان الوصول إلى المجلد العمومي لا يعمل لبعض المستخدمين، فجرّب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="b4052-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="b4052-104">الاتصال EXO PowerShell وتكوين المعلمة DefaultPublicFolderMailbox على حساب المستخدم المشكلة لمطابقة المعلمة على حساب مستخدم عامل.</span><span class="sxs-lookup"><span data-stu-id="b4052-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="b4052-105">المثال:</span><span class="sxs-lookup"><span data-stu-id="b4052-105">Example:</span></span>

<span data-ttu-id="b4052-106">الحصول على علبة البريد المستخدم | ft DefaultPublicFolderMailbox، EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="b4052-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="b4052-107">مجموعة علبة البريد مشكلةUser \<-DefaultPublicFolderMailbox قيمة من الأمر السابق></span><span class="sxs-lookup"><span data-stu-id="b4052-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="b4052-108">انتظر ساعة واحدة على الأقل حتى يسري التغيير.</span><span class="sxs-lookup"><span data-stu-id="b4052-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="b4052-109">إذا ظلت المشكلة قائمة، الرجاء اتباع [هذا الإجراء](https://aka.ms/pfcte) لاستكشاف مشاكل الوصول إلى المجلد العمومي باستخدام Outlook.</span><span class="sxs-lookup"><span data-stu-id="b4052-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>