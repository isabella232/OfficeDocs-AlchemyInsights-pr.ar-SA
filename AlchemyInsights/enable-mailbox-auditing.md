---
title: تمكين تدقيق علبة البريد
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506941"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="c8a88-102">تمكين تدقيق علبة البريد</span><span class="sxs-lookup"><span data-stu-id="c8a88-102">Enable mailbox auditing</span></span>

<span data-ttu-id="c8a88-103">لتمكين تدقيق علبة البريد لمستخدم واحد أو مؤسسة بأكملها يجب تشغيل cmdlets التالية من شل الطاقة البعيد:</span><span class="sxs-lookup"><span data-stu-id="c8a88-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="c8a88-104">**مستخدم واحد**</span><span class="sxs-lookup"><span data-stu-id="c8a88-104">**Single User**</span></span>
  
<span data-ttu-id="c8a88-105">مجموعة علبة البريد - الهوية "جين داو" -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="c8a88-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="c8a88-106">**المنظمه**</span><span class="sxs-lookup"><span data-stu-id="c8a88-106">**Organization**</span></span>
  
<span data-ttu-id="c8a88-107">الحصول على علبة البريد -ResultSize غير محدود -تصفية {RecipientTypeDetails-eq "UserMailbox"} | $true مجموعة علبة البريد -AuditEnabled</span><span class="sxs-lookup"><span data-stu-id="c8a88-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="c8a88-108">التعرف على المزيد</span><span class="sxs-lookup"><span data-stu-id="c8a88-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

