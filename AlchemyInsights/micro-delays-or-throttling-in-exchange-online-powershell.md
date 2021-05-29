---
title: التأخيرات الصغيرة أو التقييد في Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702113"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="ff217-102">التأخيرات الصغيرة أو التقييد في Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="ff217-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="ff217-103">قد تظهر التحذيرات "تم تطبيق التأخير الصغير" أو تأخيرات عند تشغيل البرامج النصية و cmdlets في Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="ff217-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="ff217-104">فيما يلي بعض الاقتراحات حول كيفية حل هذه المشكلة:</span><span class="sxs-lookup"><span data-stu-id="ff217-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="ff217-105">الرجاء تشغيل تشخيصاتنا لسترخي سياسات االتر لديك في PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ff217-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="ff217-106">سيحل هذا الحل المشكلة لمعظمهم.</span><span class="sxs-lookup"><span data-stu-id="ff217-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="ff217-107">إذا لم يتم حل المشكلة بعد، فاستخدم الوحدة النمطية Exchange Online [v2 PowerShell،](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)التي تتضمن CMDlets التي تستند إلى REST API والتي تكون أكثر أداء بشكل ملحوظ.</span><span class="sxs-lookup"><span data-stu-id="ff217-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="ff217-108">قد يكون هذا حلاً رائعًا للعديد من Get- CMDlets التي يتم استخدامها بشكل متكرر.</span><span class="sxs-lookup"><span data-stu-id="ff217-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="ff217-109">إذا كنت بحاجة إلى استخدام CMDlets غير المتناولة في الوحدة النمطية ل v2، فالرجاء الاطلاع على تشغيل [PowerShell cmdlets](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)لأعداد كبيرة من المستخدمين في Office 365 ، الذي يتحدث عن كيفية الاطلاع على حدود تقييد PowerShell في Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="ff217-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
