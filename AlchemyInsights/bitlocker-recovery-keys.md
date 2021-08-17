---
title: مفاتيح استرداد Bitlocker
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
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060051"
---
# <a name="accessing-bitlocker-recovery-keys"></a>الوصول إلى مفاتيح استرداد Bitlocker

عند تكوين إعدادات Bitlocker Intune Endpoint Protection، من الممكن تحديد ما إذا كان يجب تخزين معلومات استرداد Bitlocker في Azure Active Directory.

إذا تم تكوين هذا الإعداد، يجب أن تكون بيانات الاسترداد المخزنة مرئية لمسؤول Intune كجزء من بيانات سجل الجهاز في شفرة أجهزة Intune باستخدام طريقتين:

الأجهزة - أجهزة Azure AD -> "الجهاز" أو الأجهزة -> جميع الأجهزة -> "الجهاز" -> الاسترداد

بدلا من ذلك، إذا كان هناك وصول إداري إلى الجهاز نفسه، يمكن رؤية مفتاح الاسترداد (كلمة المرور) عن طريق تشغيل الأمر التالي من موجه أوامر مرتفع:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
إذا كان الجهاز مشفرا قبل التسجيل في Intune، فقد يكون مفتاح الاسترداد مقترن ب "حساب Microsoft" (MSA) المستخدم في تسجيل الدخول إلى الجهاز أثناء عملية OOBE. إذا كان الأمر كذلك، يجب أن يظهر الوصول إلى MSA ثم تسجيل الدخول باستخدامه الأجهزة التي تم تخزين مفاتيح  https://onedrive.live.com/recoverykey الاسترداد لها.
 
إذا تم تشفير الجهاز نتيجة التكوين من خلال نهج المجموعة المستند إلى المجال، فقد يتم تخزين معلومات الاسترداد في Active Directory المحلية.

إذا قمت بتكوين نهج حماية نقطة النهاية لتخزين مفتاح الاسترداد في Azure Active Directory ولكن لم يتم تحميل مفتاح جهاز معين، يمكنك تشغيل التحميل عن طريق تدوير مفتاح الاسترداد لهذا الجهاز من وحدة تحكم MEM. للحصول على التفاصيل، راجع [تدوير مفاتيح استرداد BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

