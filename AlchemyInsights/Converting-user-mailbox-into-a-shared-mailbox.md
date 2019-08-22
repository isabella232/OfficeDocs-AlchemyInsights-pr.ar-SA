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
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="82f30-102">تحويل علبة بريد مستخدم إلى صندوق بريد مشترك</span><span class="sxs-lookup"><span data-stu-id="82f30-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="82f30-103">يمكنك تحويل علبة بريد مستخدم إلى علبة بريد مشتركة فقط إذا كان المستخدم لديه ترخيص Exchange.</span><span class="sxs-lookup"><span data-stu-id="82f30-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="82f30-104">بعد تحويل علبة البريد، فيقوم بالظهور في قائمة المستخدمين النشطين لعلب البريد المشتركة تتضمن تلك القائمة.</span><span class="sxs-lookup"><span data-stu-id="82f30-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="82f30-105">ومع ذلك، علبة البريد المحول كما ستظهر في قائمة علب البريد المشتركة.</span><span class="sxs-lookup"><span data-stu-id="82f30-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="82f30-106">إذا حاولت تحويل علبة بريد في Exchange المشرف وفشل التحويل، مسح ذاكرة التخزين المؤقت للمستعرض الخاص بك وملفات تعريف الارتباط وحاول مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="82f30-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="82f30-107">إذا ما زال لا يعمل، حاول تحويل علبة البريد في Exchange إدارة شل بتشغيل الأمر التالي:</span><span class="sxs-lookup"><span data-stu-id="82f30-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="82f30-108">تتوفر معلومات تحويل علبة البريد أكثر في [تحويل علبة بريد مستخدم إلى صندوق بريد مشترك](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="82f30-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
