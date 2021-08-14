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
ms.openlocfilehash: cb97aa790264c23aae15fed49c353c7fb0d6209d9492c6881f1b1091fe80d7b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868521"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>التأخيرات الصغيرة أو التقييد في Exchange Online PowerShell

قد تظهر التحذيرات "تم تطبيق التأخير الصغير" أو تأخيرات عند تشغيل البرامج النصية و cmdlets في Exchange Online. فيما يلي بعض الاقتراحات حول كيفية حل هذه المشكلة:

- الرجاء تشغيل تشخيصاتنا لسترخي سياسات االتر لديك في PowerShell. سيحل هذا الحل المشكلة لمعظمهم.
- إذا لم يتم حل المشكلة بعد، فاستخدم الوحدة النمطية Exchange Online [v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)، التي تتضمن CMDlets التي تستند إلى REST API والتي تكون أكثر أداء بشكل ملحوظ. قد يكون هذا حلاً رائعًا للعديد من Get- CMDlets التي يتم استخدامها بشكل متكرر.
- إذا كنت بحاجة إلى استخدام CMDlets التي لم يتم تناولها في الوحدة النمطية v2، فالرجاء الاطلاع على تشغيل [PowerShell cmdlets](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)لأعداد كبيرة من المستخدمين في Office 365 ، الذي يتحدث عن كيفية الاجتياج حول حدود تقييد PowerShell في Exchange Online.
