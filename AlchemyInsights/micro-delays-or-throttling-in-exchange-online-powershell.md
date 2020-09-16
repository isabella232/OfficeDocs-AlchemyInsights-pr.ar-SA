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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>التأخيرات الصغيرة أو التقييد في Exchange Online PowerShell

قد تظهر التحذيرات "تم تطبيق التأخير الصغير" أو تأخيرات عند تشغيل البرامج النصية و cmdlets في Exchange Online. إليك بعض الاقتراحات المُتعلقة بهذا العنصر:

- قد تحتاج إلى محاولة استخدام [الوحدة النمطية Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)، والتي تتضمن CMDlets التي تستند إلى REST API والأداء بشكل ملحوظ. قد يكون هذا حلاً رائعًا للعديد من Get- CMDlets التي يتم استخدامها بشكل متكرر.
- إذا كنت بحاجة إلى استخدام أوامر CMDlets التي لم تتم تغطيتها في الوحدة النمطية v2 حتى الآن، فالرجاء مراجعة [تشغيل أوامر PowerShell cmdlet لعدد كبير من المستخدمين في Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)، والذي يتحدث عن كيفية الحصول على حدود التقييد في PowerShell المتوقعة في Exchange Online.
