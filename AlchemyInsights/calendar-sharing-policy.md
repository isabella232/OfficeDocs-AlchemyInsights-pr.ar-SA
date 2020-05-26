---
title: 618 سياسة مشاركة التقويم
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/26/2020
ms.locfileid: "44372986"
---
# <a name="policy-error-when-sharing-a-calendar"></a>خطأ في النهج عند مشاركة تقويم

1. قم بأحد الإجراءات التالية، حسب ما يناسب موقفك:
    - الاتصال بالتبادل عبر الإنترنت باستخدام PowerShell البعيد. لمزيد من المعلومات، راجع [الاتصال بالتبادل عبر الإنترنت باستخدام PowerShell البعيد](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - على الخادم الداخلي، افتح شل إدارة Exchange.
2. تحديد نهج المشاركة الذي تم تعيينه للمستخدم. للقيام بذلك، قم بتشغيل الأمر التالي ولاحظ النهج الذي تم إرجاعه:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. تحديث نهج المشاركة للمستخدم. لعمل ذلك، اتبع الخطوات التالية:
    - افتح مركز إدارة Exchange.
    - انقر فوق **المؤسسة**، ثم انقر نقرًا مزدوجًا على النهج الذي تم تعيينه للمستخدم ضمن **المشاركة الفردية**. هذه هي السياسة التي تم إرجاعها في الخطوة 2.
    - في صفحة قاعدة المشاركة، حدد مستوى مشاركة التقويم الذي تريد السماح به ضمن **تحديد المعلومات التي تريد مشاركتها**؛ انقر فوق **حفظ**.

لمزيد من المعلومات راجع: ["النهج لا يسمح بمنح أذونات على هذا المستوى إلى خطأ واحد أو أكثر من المستلمين (المستلمين)" عندما يحاول المستخدم مشاركة التقويم](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
