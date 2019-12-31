---
title: مفاتيح استرداد Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908802"
---
# <a name="accessing-bitlocker-recovery-keys"></a>الوصول إلى مفاتيح استرداد Bitlocker

عند تكوين إعدادات Bitlocker نهج حماية نقطه النهاية اينتوني ، فمن الممكن لتحديد ما إذا كان يجب تخزين معلومات استرداد Bitlocker في "Active Directory Azure".

إذا تم تكوين هذا الاعداد ، يجب ان تكون بيانات الاسترداد المخزنة مرئية لمسؤول اينتوني كجزء من بيانات سجل الجهاز في شفره الاجهزه اينتوني بطريقتين:

الاجهزه-أجهزه Azure AD-> "الجهاز" أو الاجهزه-> كافة الاجهزه-> "الجهاز"-> مفاتيح الاسترداد

بدلا من ذلك ، إذا كان هناك وصول اداري إلى الجهاز نفسه ، يمكن مشاهده مفتاح الاسترداد (كلمه المرور) عن طريق تشغيل الأمر التالي من موجه أوامر غير مقيد:

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
إذا تم تشفير الجهاز قبل التسجيل في اينتوني ، قد يكون مفتاح الاسترداد المقترنة مع "حساب Microsoft" (بدلا) المستخدمة لتسجيل الدخول إلى الجهاز اثناء عمليه OOBE. وإذا كانت هذه هي الحالة ، فان الوصول https://onedrive.live.com/recoverykey إلى هذا البدل وتسجيل الدخول اليه يجب ان يظهرا الاجهزه التي تم تخزين مفاتيح الاسترداد لها.
 
إذا تم تشفير الجهاز كنتيجة للتكوين من خلال نهج المجموعة المستندة إلى المجال ، فقد يتم تخزين معلومات الاسترداد في "Active Directory" الموجود في الموقع.
 

