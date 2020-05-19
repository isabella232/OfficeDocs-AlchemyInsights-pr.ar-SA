---
title: هل تحتاج إلى وضع علامة على نطاق أو مرسل بريد إلكتروني آمنًا؟
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281113"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>هل تحتاج إلى وضع علامة على نطاق أو مرسل بريد إلكتروني آمنًا؟

- لا **يوصى باستخدام قوائم المرسلين الآمنة** نظرًا لأنه يفتح مؤسستك للهجمات غير المرغوب فيها والتصيد الاحتيالي والانتحال.
- ومع ذلك، إذا كان هناك شرط عمل، **نوصي** باستخدام **[قواعد تدفق البريد](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** لهذا الغرض. تضمن إرشاداتنا مصادقة المرسل (التحقق من عدم انتحال نطاق الإرسال). **ملاحظة:** لا نوصي بإدارة الإيجابيات الزائفة باستخدام قوائم المرسلالآمنة، لأن الاستثناءات من تصفية الرسائل غير المرغوب فيها يمكن أن تفتح مؤسستك أمام هجمات الأمان. إذا تلقى المستخدم (المستخدمون) رسائل تم وضع علامة غير صحيحة عليها كبريد إلكتروني غير مرغوب فيه أو غير هام، فيرجى **[الإبلاغ عن الرسائل والملفات إلى Microsoft](https://protection.office.com/reportsubmission)**.
- **يجب تجنب** المرسلين الآمنين في Outlook أو قائمة المرسل المسموح بها أو قائمة النطاقات المسموح بها في نُهج مكافحة الرسائل غير المرغوب فيها لأن المرسلين يتجاوزون جميع الرسائل غير المرغوب فيها والخداع وحماية التصيد الاحتيالي ومصادقة المرسل (SPF وDKIM وDMARC). يتم استخدام هذا الأسلوب بشكل أفضل للاختبار المؤقت فقط.
