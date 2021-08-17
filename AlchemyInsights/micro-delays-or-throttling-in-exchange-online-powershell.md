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
ms.openlocfilehash: 2fab21f76f455815979ae162c1ce8246ad5c297e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314687"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>التأخيرات الصغيرة أو التقييد في Exchange Online PowerShell

قد تظهر التحذيرات "تم تطبيق التأخير الصغير" أو تأخيرات عند تشغيل البرامج النصية و cmdlets في Exchange Online. فيما يلي بعض الاقتراحات حول كيفية حل هذه المشكلة:

- الرجاء تشغيل تشخيصاتنا لسترخي سياسات االتر لديك في PowerShell. سيحل هذا الحل المشكلة لمعظمهم.
- إذا لم يتم حل المشكلة بعد، فاستخدم الوحدة النمطية [ل Exchange Online v2 PowerShell،](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)التي تتضمن CMDlets التي تستند إلى REST API والتي تكون أكثر أداء بشكل ملحوظ. قد يكون هذا حلاً رائعًا للعديد من Get- CMDlets التي يتم استخدامها بشكل متكرر.
- إذا كنت بحاجة إلى استخدام CMDlets غير المتناولة في الوحدة النمطية ل v2، فالرجاء الاطلاع على تشغيل [PowerShell cmdlets](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)لأعداد كبيرة من المستخدمين في Office 365 ، الذي يتحدث عن كيفية الاطلاع على حدود تقييد PowerShell في Exchange Online.
