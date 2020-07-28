---
title: لم يتم إعداد Apple MDM Certificate
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438699"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>لم يتم إعداد Apple MDM Certificate

لم يتم تكوين شهادة دفع Apple MDM (المعروفة أيضًا باسم شهادة خدمة الإعلامات المقدمة من Apple (APNS) للاشتراك. بدون تكوين شهادة دفع من Apple MDM، لن تتمكن من تسجيل أجهزة iOS و Mac OS وإدارتها. بعد إضافة الشهادة إلى Intune، يمكن للمستخدمين تثبيت تطبيق Company Portal لتسجيل أجهزة iOS الخاصة بهم.

1. حدد **"أوافق".** لإعطاء Microsoft الإذن لإرسال البيانات إلى Apple.

2. حدد **تنزيل CSR** طلب توقيع شهادة Intune المطلوب لإنشاء شهادة دفع Apple MDM. يتم استخدام الملف لطلب شهادة علاقة ثقة من "مدخل شهادات الدفع أبل".

3. حدد **إنشاء شهادة دفع MDM** للانتقال إلى مدخل شهادات الدفع التفاح. سجّل الدخول باستخدام Apple ID للشركة، ثم حدد **إنشاء شهادة**. حدد **اختيار ملف**، واستعرض إلى ملف طلب توقيع الشهادة، ثم اختر **تحميل**. في صفحة التأكيد، اختر **تنزيل** لتنزيل ملف الشهادة (.pem)، ثم احفظ الملف محلياً.
 
**ملاحظة:** ترتبط الشهادة بمعرف Apple ID المستخدم في إنشائها. وكأفضل ممارسة، استخدم Apple ID الشركة لمهام الإدارة، وتأكد من مراقبة صندوق البريد من قبل أكثر من شخص واحد أو باستخدام قائمة توزيع. لا تستخدم أبدًا Apple ID شخصيًا. استخدم نفس Apple ID لتجديد شهادة Apple Push كل 12 شهرًا.
 
4. أدخل Apple ID المستخدم لإنشاء شهادة الدفع من Apple MDM. سجل هذا المعرف كتذكير عندما تحتاج إلى تجديد الشهادة.

5. انتقل إلى ملف الشهادة (.pem) واختر **فتح**، ثم اختر **تحميل**. مع شهادة الدفع ، يمكن لـ Intune تسجيل أجهزة Apple وإدارتها.