---
title: تغيير عنوان البريد الإلكتروني الخاص بمجموعة Microsoft 365 أو Microsoft Teams
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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819067"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>تغيير عنوان البريد الإلكتروني الخاص بمجموعة Microsoft 365 أو Microsoft Teams

يمكنك تغيير عنوان البريد الإلكتروني الخاص بمجموعة Microsoft 365 أو Microsoft Teams عن طريق استخدام [مركز مسؤولي Microsoft 365](https://admin.microsoft.com/). حدد فقط المجموعة وحدد @تحرير عنوان البريد الإلكتروني. 

يمكنك أيضًا استخدام أمر EXO PowerShell التالي لتغيير عنوان SMTP الأساسي الخاص بمجموعة Microsoft 365/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

على سبيل المثال:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
