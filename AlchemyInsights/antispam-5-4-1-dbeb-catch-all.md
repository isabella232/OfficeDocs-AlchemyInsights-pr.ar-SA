---
title: مضاد البريد المزعج 5.4.1 DBEB القبض علي جميع
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672420"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>إصلاح مشكلات التسليم لرمز الخطا 550 5.4.1 رفض الوصول ترحيل

تحدث هذه [المشكلة عند التحقق لمعرفه ما إذا كان عنوان البريد الكتروني صالح لمنع الحالات الاحتياطية](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) عند إدخال شبكه 365 Office. جرب ما يلي:

1. تحديد ما إذا كانت المشكلة محدده إلى مجال بأكمله أو عنوان بريد الكتروني واحد:
    - المجال بأكمله: في بعض الأحيان يحتاج المجال إلى مزامنة; حاول [تعيين المجال إلى داخلي ثم العودة إلى مخول](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - عنوان البريد الكتروني المفرد: في بعض الأحيان يجب ان تتم مزامنة العنوان; تغيير عنوان الوكيل smtp ثم تغييره مره أخرى يمكن ان تساعد.
2. تحديد ما إذا كانت المشكلة محدده إلى مجموعه أو مجلد عمومي. بالنسبة لبعض أنواع الكائنات ، قد تحتاج إلى إنشاء يدويا في Azure Active Directory.

إذا كنت بحاجه إلى مساعده اضافيه ، يرجى فتح تذكره دعم وتحديد نطاق المشكلة (بما في ذلك نوع الكائن الذي ترسله اليه) حتى نتمكن من مساعدتك بشكل أفضل.