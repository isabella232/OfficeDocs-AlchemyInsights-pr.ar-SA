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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830020"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>التأخيرات الصغيرة أو التقييد في Exchange Online PowerShell

قد تظهر التحذيرات "تم تطبيق التأخير الصغير" أو تأخيرات عند تشغيل البرامج النصية و cmdlets في Exchange Online. إليك بعض الاقتراحات المُتعلقة بهذا العنصر:

- قد تحتاج إلى محاولة استخدام [الوحدة النمطية Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)، والتي تتضمن CMDlets التي تستند إلى REST API والأداء بشكل ملحوظ. قد يكون هذا حلاً رائعًا للعديد من Get- CMDlets التي يتم استخدامها بشكل متكرر.
- إذا كنت بحاجة إلى استخدام أوامر CMDlets التي لم تتم تغطيتها في الوحدة النمطية v2 حتى الآن، فالرجاء مراجعة [تشغيل أوامر PowerShell cmdlet لعدد كبير من المستخدمين في Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)، والذي يتحدث عن كيفية الحصول على حدود التقييد في PowerShell المتوقعة في Exchange Online.
