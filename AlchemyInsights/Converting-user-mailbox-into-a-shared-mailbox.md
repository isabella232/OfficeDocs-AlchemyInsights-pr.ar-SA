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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28273885"
---
<span data-ttu-id="3cb32-p101">يمكنك تحويل علبة بريد مستخدم إلى علبة بريد مشتركة فقط إذا كان المستخدم لديه ترخيص Exchange. بعد تحويل علبة البريد، فيقوم بالظهور في قائمة المستخدمين النشطين لعلب البريد المشتركة تتضمن تلك القائمة. ومع ذلك، علبة البريد المحول كما ستظهر في قائمة علب البريد المشتركة.</span><span class="sxs-lookup"><span data-stu-id="3cb32-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="3cb32-p102">إذا حاولت تحويل علبة بريد في Exchange المشرف وفشل التحويل، مسح ذاكرة التخزين المؤقت للمستعرض الخاص بك وملفات تعريف الارتباط وحاول مرة أخرى. إذا ما زال لا يعمل، حاول تحويل علبة البريد في Exchange إدارة شل بتشغيل الأمر التالي:</span><span class="sxs-lookup"><span data-stu-id="3cb32-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="3cb32-107">تتوفر معلومات تحويل علبة البريد أكثر في [تحويل علبة بريد مستخدم إلى صندوق بريد مشترك](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="3cb32-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
