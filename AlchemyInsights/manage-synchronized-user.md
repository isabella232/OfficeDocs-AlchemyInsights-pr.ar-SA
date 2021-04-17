---
title: إدارة المستخدم المتزامن
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823954"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>تعذر تعيين عنوان البريد الإلكتروني الأساسي أو تغيير سمات المستخدم أو إزالة/حذف مستخدم متزامن

إذا تم تمكين مزامنة الدليل بيئتك، فلا يمكن تغيير بعض سمات المستخدم أو الكائن باستخدام مركز إدارة Microsoft 365.

لإدارة المستخدمين المتزامنين وجميع سماتهم بشكل كامل، استخدم وحدة تحكم إدارة المجموعات ومستخدمي الدليل النشطين المحليين (adsiedit.msc).  

بدلا من ذلك، يمكنك تغيير المستخدمين الفرديين أو السمات للمستخدمين المتزامنين باستخدام powershell كما هو موضح في الأمثلة الشائعة هذه:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
