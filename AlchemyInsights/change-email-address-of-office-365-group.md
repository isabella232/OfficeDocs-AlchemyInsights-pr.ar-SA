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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282533"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>تغيير عنوان البريد الإلكتروني لمجموعة Microsoft 365

يمكنك تغيير عنوان البريد الإلكتروني لمجموعة Microsoft 365 باستخدام مركز المسؤول. ما عليك سوى تحديد المجموعة وتحديد عنوان البريد الإلكتروني @edit.

يمكنك أيضًا استخدام الأمر EXO PowerShell لتغيير عنوان SMTP الأساسي لمجموعة Microsoft 365:

مجموعة مجموعة موحدة <Group Name> -PrimarySmtpAddress<new SMTP Address>

المثال:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
