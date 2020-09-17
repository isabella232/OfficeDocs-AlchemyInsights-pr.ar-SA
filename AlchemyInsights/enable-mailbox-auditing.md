---
title: تمكين تدقيق علبه البريد
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806278"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="5a2c7-102">تمكين تدقيق علبه البريد</span><span class="sxs-lookup"><span data-stu-id="5a2c7-102">Enable mailbox auditing</span></span>

<span data-ttu-id="5a2c7-103">لتمكين تدقيق علبه البريد لمستخدم واحد أو مؤسسه بالبالكامل يجب تشغيل أوامر cmdlet التالية من Power Shell البعيد:</span><span class="sxs-lookup"><span data-stu-id="5a2c7-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="5a2c7-104">**مستخدم واحد**</span><span class="sxs-lookup"><span data-stu-id="5a2c7-104">**Single User**</span></span>
  
<span data-ttu-id="5a2c7-105">Set-علبه البريد-الهوية "ناجي Dow"-أوديتينابليد $true</span><span class="sxs-lookup"><span data-stu-id="5a2c7-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="5a2c7-106">**مؤسست**</span><span class="sxs-lookup"><span data-stu-id="5a2c7-106">**Organization**</span></span>
  
<span data-ttu-id="5a2c7-107">الوصول إلى علبه البريد-ريسولتسيزي-تصفيه غير محدوده {ريسيبينتيبيديتايلس "أوسيرمايلبوكس"} | Set-علبه البريد-أوديتينابليد $true</span><span class="sxs-lookup"><span data-stu-id="5a2c7-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="5a2c7-108">التعرف على المزيد</span><span class="sxs-lookup"><span data-stu-id="5a2c7-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

