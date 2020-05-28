---
title: إدارة المستخدم المتزامن
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407337"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>غير قادر على تعيين عنوان البريد الإلكتروني الأساسي أو تغيير سمات المستخدم أو إزالة/حذف مستخدم متزامن

إذا تم تمكين مزامنة الدليل للبيئة الخاصة بك، لا يمكن تغيير بعض سمات المستخدم أو الكائن باستخدام مركز إدارة Microsoft 365.

لإدارة المستخدمين المتزامنين وجميع سماتهم بشكل كامل، استخدم مستخدمي الدليل النشط المحلي ووحدة تحكم إدارة المجموعات (adsiedit.msc).  

بدلاً من ذلك، يمكنك تغيير المستخدمين الفرديين أو السمات للمستخدمين المتزامنين باستخدام powershell مثل هو موضح في هذه الأمثلة الشائعة: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
