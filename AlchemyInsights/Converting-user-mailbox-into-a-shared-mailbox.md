---
title: تحويل علبة بريد مستخدم إلى علبة بريد مشتركة؟
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29455694"
---
يمكنك تحويل علبة بريد مستخدم إلى علبة بريد مشتركة فقط إذا كان المستخدم لديه ترخيص Exchange. بعد تحويل علبة البريد، فيقوم بالظهور في قائمة المستخدمين النشطين لعلب البريد المشتركة تتضمن تلك القائمة. ومع ذلك، علبة البريد المحول كما ستظهر في قائمة علب البريد المشتركة. 
  
إذا حاولت تحويل علبة بريد في Exchange المشرف وفشل التحويل، مسح ذاكرة التخزين المؤقت للمستعرض الخاص بك وملفات تعريف الارتباط وحاول مرة أخرى. إذا ما زال لا يعمل، حاول تحويل علبة البريد في Exchange إدارة شل بتشغيل الأمر التالي:
  
```
Set-Mailbox -Type Shared
```

تتوفر معلومات تحويل علبة البريد أكثر في [تحويل علبة بريد مستخدم إلى صندوق بريد مشترك](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
