---
title: تعيين الردود التلقائية لعبة البريد
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788869"
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
