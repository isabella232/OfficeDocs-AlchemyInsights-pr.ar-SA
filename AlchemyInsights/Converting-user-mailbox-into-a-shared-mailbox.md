---
title: تحويل علبة بريد مستخدم إلى علبة بريد مشتركة؟
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496386"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>تحويل علبة بريد مستخدم إلى صندوق بريد مشترك

يمكنك تحويل علبة بريد مستخدم إلى علبة بريد مشتركة فقط إذا كان المستخدم لديه ترخيص Exchange. بعد تحويل علبة البريد، فيقوم بالظهور في قائمة المستخدمين النشطين لعلب البريد المشتركة تتضمن تلك القائمة. ومع ذلك، علبة البريد المحول كما ستظهر في قائمة علب البريد المشتركة. 
  
إذا حاولت تحويل علبة بريد في Exchange المشرف وفشل التحويل، مسح ذاكرة التخزين المؤقت للمستعرض الخاص بك وملفات تعريف الارتباط وحاول مرة أخرى. إذا ما زال لا يعمل، حاول تحويل علبة البريد في Exchange إدارة شل بتشغيل الأمر التالي:
  
```
Set-Mailbox -Type Shared
```

تتوفر معلومات تحويل علبة البريد أكثر في [تحويل علبة بريد مستخدم إلى صندوق بريد مشترك](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
