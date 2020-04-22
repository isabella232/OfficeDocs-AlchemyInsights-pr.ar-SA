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
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703558"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="d6aed-102">تمكين تدقيق علبة البريد</span><span class="sxs-lookup"><span data-stu-id="d6aed-102">Enable mailbox auditing</span></span>

<span data-ttu-id="d6aed-103">لتمكين تدقيق علبة البريد لمستخدم واحد أو مؤسسة بأكملها يجب تشغيل cmdlets التالية من شل الطاقة البعيد:</span><span class="sxs-lookup"><span data-stu-id="d6aed-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="d6aed-104">**مستخدم واحد**</span><span class="sxs-lookup"><span data-stu-id="d6aed-104">**Single User**</span></span>
  
<span data-ttu-id="d6aed-105">مجموعة علبة البريد - الهوية "جين داو" -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="d6aed-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="d6aed-106">**المنظمه**</span><span class="sxs-lookup"><span data-stu-id="d6aed-106">**Organization**</span></span>
  
<span data-ttu-id="d6aed-107">الحصول على علبة البريد -ResultSize غير محدود -تصفية {RecipientTypeDetails-eq "UserMailbox"} | $true مجموعة علبة البريد -AuditEnabled</span><span class="sxs-lookup"><span data-stu-id="d6aed-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="d6aed-108">التعرف على المزيد</span><span class="sxs-lookup"><span data-stu-id="d6aed-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

