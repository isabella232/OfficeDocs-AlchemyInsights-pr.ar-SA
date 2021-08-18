---
title: 2681 Attack Simulator في Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: f6e221cc82a1b707f6acc457cb78db743521d859
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325058"
---
# <a name="attack-simulator-in-microsoft-365"></a>محاكي الهجوم في Microsoft 365

- هل تفتقد "محاكي الهجوم"؟ يتطلب "محاكي الهجوم" **وجود Microsoft Defender Office 365 2** أو Office 365 Enterprise **E5.** لا يتم **تضمين** محاكي الهجوم في Microsoft Defender Office 365 1 أو Office 365 Enterprise E3 أو أي اشتراكات Microsoft 365 Apps for business اشتراكات.

- يتطلب الحساب الذي تستخدمه لشن هجمات محاكاة أذونات مسؤول عام أو مسؤول أمان ومصادقة متعددة العوامل (MFA). لمزيد من المعلومات حول متطلبات "محاكي الهجمات"، راجع [هذا الموضوع](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- أشياء مهمة يجب معرفتها حول عمليات محاكاة هجوم **"القوة الغاشمة لكلمة** المرور":

  - إذا تم تمكين المصادقة MFA للحساب الهدف وكان تخمين كلمة المرور صحيحا، لن يظهر الحساب كمعرض للخطر (سيكون عامل المصادقة الثاني غير مكتمل).

  - لا يمكن أن يزيد حجم ملف كلمة المرور عن 10 مبايت. استخدم كلمة مرور واحدة لكل سطر، ثم قم بتضمين سطر فارغ (إرجاع السطر) بعد كلمة المرور الأخيرة في القائمة.

- أشياء مهمة يجب معرفتها حول عمليات محاكاة **"التصيد الاحتيالي من أجل** التصيد الاحتيالي":

  - حسب التصميم، لا يمكنك توفير قيمة مخصصة ل URL خادم تسجيل الدخول إلى التصيد **الاحتيالي**.

  - إذا استخدم المستلم [](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) الميزة الإضافية تمكين رسالة التقرير للتقارير حول الرسالة على أنها تصيد احتيالي، فقد لا تتلقى تنبيهات للرسالة (لأن هذا هجوم محاكاة).

- التقارير: بعد اكتمال الهجوم المحاكاة، يمكنك النقر **فوق** تفاصيل الهجوم للاطلاع على التقرير.

- للحصول على إرشادات مفصلة وميزات جديدة في "محاكي الهجوم"، راجع [محاكي](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)الهجوم في Microsoft 365 .
