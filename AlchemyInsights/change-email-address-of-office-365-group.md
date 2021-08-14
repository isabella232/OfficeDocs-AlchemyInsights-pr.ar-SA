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
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930716"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>تغيير عنوان البريد الإلكتروني لمجموعة Microsoft 365

يمكنك تغيير عنوان البريد الإلكتروني لمجموعة Microsoft 365 باستخدام مركز الإدارة. حدد فقط المجموعة وحدد @تحرير عنوان البريد الإلكتروني. 

يمكنك أيضا استخدام اتباع الأمر EXO PowerShell لتغيير عنوان SMTP الأساسي لمجموعة Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

على سبيل المثال:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
