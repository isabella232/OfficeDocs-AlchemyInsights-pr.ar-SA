---
title: إرسال كمجموعه Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871580"
---
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="82318-102">إرسال كمجموعه Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="82318-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="82318-103">يمكنك تعيين أذونات "إرسال ك" للسماح لمستخدمين محددين بإرسال الرسائل كمجموعه Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="82318-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="82318-104">الاتصال ب Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="82318-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="82318-105">قم بتنفيذ الأمر التالي:</span><span class="sxs-lookup"><span data-stu-id="82318-105">Run the following command:</span></span>  

    <span data-ttu-id="82318-106">الوظائف الاضافيه ريسيبينتبيرميشن `<GroupName>` -الموثوق بها `<MailboxName>` -أكسيسرايتس سندس</span><span class="sxs-lookup"><span data-stu-id="82318-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="82318-107">لمزيد من المعلومات ، راجع [السماح للأعضاء بالإرسال بالنيابة عن مجموعه أو إرسالها](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="82318-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>