---
title: تغيير عنوان البريد الإلكتروني لمجموعة Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580644"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>تغيير عنوان البريد الإلكتروني لمجموعة Microsoft 365

يمكنك تغيير عنوان البريد الإلكتروني لمجموعة Microsoft 365 باستخدام مركز المسؤول. ما عليك سوى تحديد المجموعة وتحديد عنوان البريد الإلكتروني @edit.

يمكنك أيضًا استخدام الأمر EXO PowerShell لتغيير عنوان SMTP الأساسي لمجموعة Microsoft 365:

مجموعة مجموعة موحدة <Group Name> -PrimarySmtpAddress<new SMTP Address>

المثال:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
