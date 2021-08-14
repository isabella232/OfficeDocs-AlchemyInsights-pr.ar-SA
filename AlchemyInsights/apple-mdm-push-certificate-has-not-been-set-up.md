---
title: لم يتم إعداد شهادة الدفع من Apple MDM
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 4f8e3502a7be35b5579ec1436852fe2bff9b1316891c7a9020f6f5f4767b3d88
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931509"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>لم يتم إعداد شهادة الدفع من Apple MDM

لم يتم تكوين شهادة Apple MDM Push (المعروفة أيضا بشهادة خدمة الإعلامات من Apple (APNS) لاشتراكك. إذا لم يتم تكوين شهادة الدفع من Apple MDM، لن تتمكن من تسجيل أجهزة iOS و Mac OS وإدارتها. بعد إضافة الشهادة إلى Intune، يمكن للمستخدمين تثبيت Company Portal لتسجيل أجهزة iOS الخاصة بهم.

1. حدد **"أوافق".** لإعطاء Microsoft الإذن لإرسال البيانات إلى Apple.

2. حدد **تنزيل CSR** طلب توقيع شهادة Intune المطلوب لإنشاء شهادة دفع Apple MDM. يتم استخدام الملف لطلب شهادة علاقة ثقة من مدخل شهادات Apple Push.

3. حدد **إنشاء شهادة الدفع MDM** الخاصة بك للذهاب إلى مدخل شهادات Apple Push. سجل الدخول باستخدام Apple ID الخاص بالشركة، ثم حدد **إنشاء شهادة**. حدد **اختيار ملف**، استعرض إلى ملف طلب توقيع الشهادة، ثم اختر **Upload**. في صفحة التأكيد، اختر **تنزيل** لتنزيل ملف الشهادة (.pem)، واحفظ الملف محليا.
 
**ملاحظة:** الشهادة مقترنة بم ID Apple المستخدم لإنشاءها. كأفضل ممارسة، استخدم Apple ID الخاص بالشركة لمهام الإدارة، وتأكد من مراقبة علبة البريد من قبل أكثر من شخص واحد أو باستخدام قائمة توزيع. لا تستخدم أبدا "Apple ID" الشخصي. استخدم نفس "Apple ID" لتجديد "شهادة الدفع من Apple" كل 12 شهرا.
 
4. أدخل "Apple ID" المستخدم لإنشاء شهادة دفع Apple MDM. سجل هذا الم ID كتذكير عندما تحتاج إلى تجديد الشهادة.

5. انتقل إلى ملف الشهادة (.pem)، واختر **فتح**، ثم اختر **Upload**. باستخدام شهادة الدفع، يمكن ل Intune تسجيل أجهزة Apple وإدارتها.