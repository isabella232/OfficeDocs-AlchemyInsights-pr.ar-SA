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
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="64f77-102">تغيير عنوان البريد الإلكتروني لمجموعة Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="64f77-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="64f77-103">يمكنك تغيير عنوان البريد الإلكتروني لمجموعة Microsoft 365 باستخدام مركز المسؤول.</span><span class="sxs-lookup"><span data-stu-id="64f77-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="64f77-104">ما عليك سوى تحديد المجموعة وتحديد عنوان البريد الإلكتروني @edit.</span><span class="sxs-lookup"><span data-stu-id="64f77-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="64f77-105">يمكنك أيضًا استخدام الأمر EXO PowerShell لتغيير عنوان SMTP الأساسي لمجموعة Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="64f77-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="64f77-106">مجموعة مجموعة موحدة <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="64f77-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="64f77-107">المثال:</span><span class="sxs-lookup"><span data-stu-id="64f77-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
