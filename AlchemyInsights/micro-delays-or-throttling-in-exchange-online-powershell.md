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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>التأخيرات الصغيرة أو التقييد في Exchange Online PowerShell

قد تظهر التحذيرات "تم تطبيق التأخير الصغير" أو تأخيرات عند تشغيل البرامج النصية و cmdlets في Exchange Online. فيما يلي بعض الاقتراحات حول كيفية حل هذه المشكلة:

- الرجاء تشغيل تشخيصاتنا لسترخي سياسات االتر لديك في PowerShell. سيحل هذا الحل المشكلة لمعظمهم.
- إذا لم يتم حل المشكلة بعد، فاستخدم الوحدة النمطية Exchange Online [v2 PowerShell،](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)التي تتضمن CMDlets التي تستند إلى REST API والتي تكون أكثر أداء بشكل ملحوظ. قد يكون هذا حلاً رائعًا للعديد من Get- CMDlets التي يتم استخدامها بشكل متكرر.
- إذا كنت بحاجة إلى استخدام CMDlets غير المتناولة في الوحدة النمطية ل v2، فالرجاء الاطلاع على تشغيل [PowerShell cmdlets](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)لأعداد كبيرة من المستخدمين في Office 365 ، الذي يتحدث عن كيفية الاطلاع على حدود تقييد PowerShell في Exchange Online.
