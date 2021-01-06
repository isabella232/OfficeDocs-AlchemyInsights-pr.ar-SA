---
title: تغيير عنوان البريد الإلكتروني الخاص بمجموعة Microsoft 365 أو Microsoft Teams
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
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756544"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>تغيير عنوان البريد الإلكتروني الخاص بمجموعة Microsoft 365 أو Microsoft Teams

يمكنك تغيير عنوان البريد الإلكتروني الخاص بمجموعة Microsoft 365 أو Microsoft Teams عن طريق استخدام [مركز مسؤولي Microsoft 365](https://admin.microsoft.com/). حدد فقط المجموعة وحدد @تحرير عنوان البريد الإلكتروني. 

يمكنك أيضًا استخدام أمر EXO PowerShell التالي لتغيير عنوان SMTP الأساسي الخاص بمجموعة Microsoft 365/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

على سبيل المثال:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
