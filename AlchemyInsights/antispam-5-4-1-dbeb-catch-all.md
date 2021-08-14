---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932264"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>إصلاح مشاكل التسليم لرمز الخطأ 550 5.4.1 رفض الوصول إلى الترحيل

تحدث هذه المشكلة عند التحقق لمعرفة ما إذا كان عنوان البريد الإلكتروني [صالحا](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) لمنع حدوث ارتداد عند الدخول إلى شبكة Microsoft. جرب ما يلي:

1. تحديد ما إذا كانت المشكلة خاصة لمجال بأكمله أو عنوان بريد إلكتروني واحد:
    - المجال بأكمله: يحتاج المجال في بعض الأحيان إلى مزامنة؛ حاول [تعيين المجال إلى داخلي ثم العودة إلى موثوق](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - عنوان بريد إلكتروني واحد: في بعض الأحيان يجب مزامنة العنوان؛ قد يساعدك تغيير عنوان وكيل smtp ثم تغييره مرة أخرى.
2. تحديد ما إذا كانت المشكلة خاصة ب مجموعة أو مجلد عمومي. بالنسبة لبعض أنواع العناصر، قد تحتاج الكائنات إلى إنشاء يدويا في Azure Active Directory.

إذا كنت بحاجة إلى مساعدة إضافية، فيرجى فتح تذكرة دعم وتحديد نطاق المشكلة (بما في ذلك نوع الكائن الذي ترسل إليه) حتى يمكننا مساعدتك بشكل أفضل.