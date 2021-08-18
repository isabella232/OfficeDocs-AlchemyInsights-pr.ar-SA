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
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114745"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>تعذر تعيين عنوان البريد الإلكتروني الأساسي أو تغيير سمات المستخدم أو إزالة/حذف مستخدم متزامن

إذا تم تمكين مزامنة الدليل لبيئة، فلا يمكن تغيير بعض سمات المستخدم أو الكائن باستخدام مركز مسؤولي Microsoft 365.

لإدارة المستخدمين المتزامنين وجميع سماتهم بشكل كامل، استخدم وحدة تحكم إدارة المجموعات ومستخدمي الدليل النشطين المحليين (adsiedit.msc).  

بدلا من ذلك، يمكنك تغيير المستخدمين الفرديين أو السمات للمستخدمين المتزامنين باستخدام powershell كما هو موضح في الأمثلة الشائعة هذه:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
