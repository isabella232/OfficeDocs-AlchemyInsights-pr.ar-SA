---
title: تعيين الردود التلقائية لعبة البريد
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
- "9000761"
- "3514"
ms.openlocfilehash: 03c530e7ce5f00fce2222cf9993930b97e5a2818
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715116"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>تعيين الردود التلقائية لعلبة بريد المستخدم

**الطريقة 1**

1. سجّل الدخول إلى مدخل Microsoft 365.

2. انتقل إلى **المستخدمون > المستخدمون النشطاء** (أو **المجموعات > علب البريد المشتركة** إذا قمت بتعيين ذلك في علبة بريد مشتركة).

3. حدد المستخدم الذي يمتلك علبة بريد Microsoft Exchange.

4. في القائمة الثانوية على اليسار، انتقل إلى **إعدادات البريد > الردود التلقائية** (إذا كانت علبة البريد مشتركة، فما عليك سوى النقر فوق **الردود التلقائية** في القائمة الثانوية).

**الطريقة 2**

1. سجّل الدخول إلى مدخل مسؤولي Microsoft 365 باستخدام بيانات اعتماد المسؤول.

2. قم بتوسيع **مراكز المسؤولين** ثم انقر فوق **Exchange**.

3. انقر فوق الصورة الموجودة أعلى الزاوية اليسرى وانقر فوق **مستخدم آخر** ثم حدد علبة بريد المستخدم المراد تغييرها.

4. على الجانب الأيمن، حدد **الخيارات** وانقر فوق **تنظيم البريد الإلكتروني** ثم انقر فوق **الردود التلقائية.**

**الطريقة 3**

قم بتشغيل أمر cmdlet التالي في Exchange Online PowerShell:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

للحصول على مزيد من المعلومات حول أمر cmdlet هذا، اطلع على [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
