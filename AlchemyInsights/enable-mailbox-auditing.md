---
title: تمكين تدقيق علبة البريد
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736240"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="b3c39-102">تمكين تدقيق علبة البريد</span><span class="sxs-lookup"><span data-stu-id="b3c39-102">Enable mailbox auditing</span></span>

<span data-ttu-id="b3c39-103">لتمكين "تدقيق علبة البريد" لمستخدم واحد أو مؤسسة بأكملها cmdlets يجب تشغيل cmdlets التالية من Shell الطاقة عن بعد:</span><span class="sxs-lookup"><span data-stu-id="b3c39-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="b3c39-104">**مستخدم واحد**</span><span class="sxs-lookup"><span data-stu-id="b3c39-104">**Single User**</span></span>
  
<span data-ttu-id="b3c39-105">مجموعة علبة البريد-الهوية "جين داو" -$true</span><span class="sxs-lookup"><span data-stu-id="b3c39-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="b3c39-106">**المنظمه**</span><span class="sxs-lookup"><span data-stu-id="b3c39-106">**Organization**</span></span>
  
<span data-ttu-id="b3c39-107">الحصول على علبة البريد-ResultSize غير محدود-تصفية {ريسينتيبيتفاصيل-مكافئ "أوسيرميلبوكس"} | مجموعة علبة البريد-$true التدقيق</span><span class="sxs-lookup"><span data-stu-id="b3c39-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="b3c39-108">التعرف على المزيد</span><span class="sxs-lookup"><span data-stu-id="b3c39-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

