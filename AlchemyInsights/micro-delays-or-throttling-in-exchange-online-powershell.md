---
title: التأخيرات الصغيرة أو التقييد في Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 55844747be27ea4ff8f538492e576195b3a5f0bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743817"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="09e6e-102">التأخيرات الصغيرة أو التقييد في Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="09e6e-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="09e6e-103">قد تظهر التحذيرات "تم تطبيق التأخير الصغير" أو تأخيرات عند تشغيل البرامج النصية و cmdlets في Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="09e6e-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="09e6e-104">إليك بعض الاقتراحات المُتعلقة بهذا العنصر:</span><span class="sxs-lookup"><span data-stu-id="09e6e-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="09e6e-105">قد تحتاج إلى محاولة استخدام [الوحدة النمطية Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)، والتي تتضمن CMDlets التي تستند إلى REST API والأداء بشكل ملحوظ.</span><span class="sxs-lookup"><span data-stu-id="09e6e-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="09e6e-106">قد يكون هذا حلاً رائعًا للعديد من Get- CMDlets التي يتم استخدامها بشكل متكرر.</span><span class="sxs-lookup"><span data-stu-id="09e6e-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="09e6e-107">إذا كنت بحاجة إلى استخدام أوامر CMDlets التي لم تتم تغطيتها في الوحدة النمطية v2 حتى الآن، فالرجاء مراجعة [تشغيل أوامر PowerShell cmdlet لعدد كبير من المستخدمين في Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)، والذي يتحدث عن كيفية الحصول على حدود التقييد في PowerShell المتوقعة في Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="09e6e-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
