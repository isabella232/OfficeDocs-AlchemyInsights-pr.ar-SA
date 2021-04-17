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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="af56f-102">تغيير عنوان البريد الإلكتروني لمجموعة Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="af56f-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="af56f-103">يمكنك تغيير عنوان البريد الإلكتروني لمجموعة Microsoft 365 باستخدام مركز الإدارة.</span><span class="sxs-lookup"><span data-stu-id="af56f-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="af56f-104">حدد فقط المجموعة وحدد @تحرير عنوان البريد الإلكتروني. </span><span class="sxs-lookup"><span data-stu-id="af56f-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="af56f-105">يمكنك أيضا استخدام اتباع الأمر EXO PowerShell لتغيير عنوان SMTP الأساسي لمجموعة Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="af56f-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="af56f-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="af56f-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="af56f-107">على سبيل المثال:</span><span class="sxs-lookup"><span data-stu-id="af56f-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
