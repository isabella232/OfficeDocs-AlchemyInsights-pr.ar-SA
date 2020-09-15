---
title: نهج مشاركه تقويم 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684217"
---
# <a name="policy-error-when-sharing-a-calendar"></a>خطا في النهج عند مشاركه تقويم

1. قم بواحد مما يلي ، بما يتناسب مع حالتك:
    - الاتصال ب Exchange Online باستخدام PowerShell البعيد. لمزيد من المعلومات ، راجع [الاتصال ب Exchange Online باستخدام PowerShell البعيد](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - علي الخادم المحلي ، افتح Exchange Management Shell.
2. تحديد نهج المشاركة الذي تم تعيينه إلى المستخدم. للقيام بذلك ، قم بتشغيل الأمر التالي ولاحظ ان النهج ارجع:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. تحديث نهج المشاركة للمستخدم. لعمل ذلك، اتبع الخطوات التالية:
    - افتح مركز أداره Exchange.
    - انقر فوق **المؤسسة**، ثم انقر نقرا مزدوجا فوق النهج الذي تم تعيينه إلى المستخدم ضمن **المشاركة الفردية**. هذا هو النهج الذي تم إرجاعه في الخطوة 2.
    - في صفحه قاعده المشاركة ، حدد مستوي مشاركه التقويم الذي تريد السماح به ضمن **تحديد المعلومات التي تريد مشاركتها**؛ انقر فوق **حفظ**.

لمزيد من المعلومات ، راجع: ["لا يسمح النهج بمنح الأذونات الموجودة في هذا المستوي إلى رسالة واحده أو أكثر من المستلمين" عند محاولة المستخدم مشاركه التقويم](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
