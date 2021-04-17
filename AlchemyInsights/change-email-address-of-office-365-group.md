---
title: تغيير عنوان البريد الإلكتروني لمجموعة Microsoft 365
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
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819031"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>تغيير عنوان البريد الإلكتروني لمجموعة Microsoft 365

يمكنك تغيير عنوان البريد الإلكتروني لمجموعة Microsoft 365 باستخدام مركز الإدارة. حدد فقط المجموعة وحدد @تحرير عنوان البريد الإلكتروني. 

يمكنك أيضا استخدام اتباع الأمر EXO PowerShell لتغيير عنوان SMTP الأساسي لمجموعة Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

على سبيل المثال:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
