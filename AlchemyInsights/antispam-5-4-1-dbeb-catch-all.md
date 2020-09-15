---
title: أنتيسبام 5.4.1 دبيب catch-الكل
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717348"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>إصلاح مشاكل التسليم لرمز الخطا 550 5.4.1 الوصول إلى الناقل الكهربائي

تحدث هذه [المشكلة عند التحقق مما إذا كان عنوان البريد الكتروني صالحا لمنع البونسيباكس](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) عند إدخال شبكه Microsoft. جرب ما يلي:

1. تحديد ما إذا كانت المشكلة خاصه بمجال كامل أو عنوان بريد الكتروني واحد:
    - المجال بالبالكامل: يجب ان تتم مزامنة المجال في بعض الأحيان ؛ حاول [تعيين المجال إلى داخلي ثم عد إلى مخول](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - عنوان البريد الكتروني الفردي: يجب ان تتم مزامنة العنوان في بعض الأحيان ؛ يمكنك تغيير عنوان وكيل smtp ثم تغييره مره أخرى.
2. تحديد ما إذا كانت المشكلة خاصه بمجموعه أو مجلد عمومي. بالنسبة إلى بعض أنواع الكائنات ، قد تحتاج إلى إنشاء الكائنات يدويا في Azure Active directory.

إذا كنت بحاجه إلى مزيد من المساعدة ، يرجى فتح بطاقة دعم وتحديد نطاق المشكلة (بما في ذلك نوع الكائن الذي ترسله اليه) بحيث يمكننا مساعدتك بشكل أفضل.