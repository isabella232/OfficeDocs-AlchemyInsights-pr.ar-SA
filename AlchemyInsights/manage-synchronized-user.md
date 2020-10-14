---
title: أداره المستخدم المتزامن
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451387"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>تعذر تعيين عنوان البريد الكتروني الأساسي أو تغيير سمات المستخدم أو أزاله/حذف مستخدم متزامن

إذا تم تمكين مزامنة الدليل لبيئتك ، فلا يمكن تغيير بعض سمات المستخدمين أو الكائنات باستخدام مركز أداره Microsoft 365.

لأداره المستخدمين المتزامنين وكل السمات الخاصة بهم بالبالكامل ، استخدم "وحده التحكم في أداره المستخدمين المحليين" ل active directory (أدسييديت).  

بدلا من ذلك ، يمكنك تغيير المستخدمين الفرديين أو السمات لمستخدمين متزامنين باستخدام powershell كما هو مبين في هذه الامثله الشائعة:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
