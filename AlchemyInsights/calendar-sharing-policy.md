---
title: نهج مشاركة التقويم 618
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
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091570"
---
# <a name="policy-error-when-sharing-a-calendar"></a>خطأ النهج عند مشاركة تقويم

1. القيام بوا واحد من الإجراءات التالية، بما يلائم وضعك:
    - الاتصال Exchange Online باستخدام Remote PowerShell. لمزيد من المعلومات، راجع الاتصال [Exchange Online Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - على الخادم في الموقع، افتح Exchange Management Shell.
2. تحديد نهج المشاركة المعين إلى المستخدم. للقيام بذلك، يمكنك تشغيل الأمر التالي ولاحظ أن النهج تم إرجاعه:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. تحديث نهج المشاركة للمستخدم. لعمل ذلك، اتبع الخطوات التالية:
    - افتح Exchange الإدارة.
    - انقر **فوق** المؤسسة ، ثم انقر نقرا مزدوجا فوق النهج المعين إلى المستخدم ضمن **المشاركة الفردية**. هذا هو النهج الذي تم إرجاعه في الخطوة 2.
    - في صفحة قاعدة المشاركة، حدد مستوى مشاركة التقويم الذي تريد السماح به ضمن **تحديد المعلومات التي تريد مشاركتها**؛ انقر فوق **حفظ**.

لمزيد من المعلومات، راجع: "لا يسمح النهج بمنح أذونات على هذا المستوى لخطأ واحد أو أكثر من المستلمين [(المستلمين)](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)عندما يحاول المستخدم مشاركة التقويم.
