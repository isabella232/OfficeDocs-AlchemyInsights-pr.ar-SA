---
title: مكافحة البريد المزعج 5.4.1 DBEB الصيد للجميع
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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707898"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>إصلاح مشكلات التسليم لرمز الخطأ 550 5.4.1 ترحيل الوصول رفض

تحدث هذه المشكلة عند [التحقق لمعرفة ما إذا كان عنوان البريد الإلكتروني صالحلمنع الارتدادعند](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) إدخال شبكة Microsoft. جرّب ما يلي:

1. تحديد ما إذا كانت المشكلة خاصة بنطاق بأكمله أو عنوان بريد إلكتروني واحد:
    - المجال بأكمله: في بعض الأحيان يجب مزامنة المجال; حاول [تعيين المجال إلى داخلي ثم العودة إلى "موثوقة".](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - عنوان بريد إلكتروني واحد: في بعض الأحيان يجب مزامنة العنوان. تغيير عنوان وكيل smtp ومن ثم تغييره مرة أخرى يمكن أن يساعد.
2. تحديد ما إذا كانت المشكلة خاصة بمجموعة أو مجلد عام. بالنسبة لبعض أنواع الكائنات، قد تحتاج الكائنات إلى إنشاء يدوياً في Azure Active Directory.

إذا كنت بحاجة إلى مساعدة إضافية، يرجى فتح تذكرة دعم وتحديد نطاق المشكلة (بما في ذلك نوع الكائن الذي ترسل إليه) حتى نتمكن من مساعدتك بشكل أفضل.