---
title: هل تحتاج إلى وضع علامة آمن على مجال أو مرسل بريد إلكتروني؟
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7058b6419e52fce94f3359d0bd8e1d67c5aa5ef6743abf4ed39f45bad49e1d07
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025597"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>هل تحتاج إلى وضع علامة آمن على مجال أو مرسل بريد إلكتروني؟

- لا يوصى باستخدام قوائم **المرسلين** الآمنة لأنها تفتح مؤسستك لهجمات البريد العشوائي والتصيد الاحتيالي والخادعة.
- ومع ذلك، إذا كان هناك  أحد متطلبات العمل، فإننا نوصي باستخدام **["Flow البريد"](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** لهذا الأمر. تضمن إرشاداتنا مصادقة المرسل (التحقق من أن مجال الإرسال لا يتم الانتحال). **ملاحظة:** لا نوصي بإدارة الإيجابيات الخاطئة باستخدام قوائم المرسلين الآمنة، لأن الاستثناءات من تصفية البريد العشوائي يمكن أن تفتح مؤسستك لهجمات الأمان. إذا تلقى المستخدم (المستخدمون) رسائل تم وضع علامة عليها بشكل غير صحيح كبريد عشوائي أو بريد إلكتروني غير هام، فيرجى الإبلاغ عن الرسائل والملفات **[إلى Microsoft](https://protection.office.com/reportsubmission)**.
- خزينة يجب تجنب المرسلين في Outlook أو قائمة المرسلين المسموح بها أو  قائمة المجالات المسموح بها في سياسات مكافحة البريد العشوائي لأن المرسلين يتجاوزون كل البريد العشوائي والخادع والحماية من التصيد الاحتيالي ومصادقة المرسل (SPF و DKIM و DMARC). يتم استخدام هذا الأسلوب بشكل أفضل للاختبار المؤقت فقط.
- التحقق من صحة تجاوز تقييم Antispam لبريد إلكتروني معين من خلال التحقق من رأس الرسالة "X-Forefront-Antispam-Report" (SFV:SFE، SFV:SKA، SFV:SKN)، راجع رؤوس رسائل مكافحة البريد العشوائي **[.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- نظرا لأن Microsoft تريد [](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)الحفاظ على أمان عملائنا بشكل افتراضي، لا يتم تطبيق بعض عمليات تجاوز المستأجر للبرامج الضارة والتصيد الاحتيالي عالي الثقة. تتضمن هذه التجاوزات: o قوائم المرسلين المسموح بها أو قوائم المجالات المسموح بها (سياسات مكافحة البريد العشوائي) o Outlook خزينة المرسلون o قائمة السماح باستخدام IP (تصفية الاتصال) 
- التجاوز الوحيد الذي يسمح برسالة التصيد الاحتيالي عالية الثقة لتجاوز التصفية هو Exchange تدفق البريد (المعروفة أيضا بقواعد النقل). لاستخدام قواعد تدفق البريد لتجاوز التصفية، راجع استخدام قواعد تدفق البريد لتعيين مستوى الثقة في البريد العشوائي **[(SCL) في الرسائل](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**.