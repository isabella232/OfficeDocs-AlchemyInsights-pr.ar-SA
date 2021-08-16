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
ms.openlocfilehash: b173c6eb3bbbd1beba3b59878ae12bbe7684d0447a16fef746e5b97b82349e53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065271"
---
# <a name="attack-simulator-in-microsoft-365"></a>محاكي الهجوم في Microsoft 365

- هل تفتقد "محاكي الهجوم"؟ يتطلب محاكي الهجوم **وجود Microsoft Defender Office 365 2** أو Office 365 Enterprise **E5**. لا يتم **تضمين** محاكي الهجوم في Microsoft Defender Office 365 1 أو Office 365 Enterprise E3 أو أي اشتراكات Microsoft 365 Apps for business اشتراكات.

- يتطلب الحساب الذي تستخدمه لشن هجمات محاكاة أذونات المسؤول العام أو مسؤول الأمان والمصادقة متعددة العوامل (MFA). لمزيد من المعلومات حول متطلبات "محاكي الهجمات"، راجع [هذا الموضوع](/microsoft-365/security/office-365-security/attack-simulator).

- أشياء مهمة يجب معرفتها حول عمليات محاكاة هجوم **"القوة الغاشمة لكلمة** المرور":

  - إذا تم تمكين المصادقة MFA للحساب الهدف وكان تخمين كلمة المرور صحيحا، لن يظهر الحساب كمعرض للخطر (سيكون عامل المصادقة الثاني غير مكتمل).

  - لا يمكن أن يزيد حجم ملف كلمة المرور عن 10 مبايت. استخدم كلمة مرور واحدة لكل سطر، ثم قم بتضمين سطر فارغ (إرجاع السطر) بعد كلمة المرور الأخيرة في القائمة.

- أشياء مهمة يجب معرفتها حول عمليات محاكاة **"التصيد الاحتيالي من أجل** التصيد الاحتيالي":

  - حسب التصميم، لا يمكنك توفير قيمة مخصصة ل URL خادم تسجيل الدخول إلى التصيد **الاحتيالي**.

  - إذا استخدم المستلم [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) الميزة الإضافية تمكين رسالة التقرير للتقارير حول الرسالة على أنها تصيد احتيالي، فقد لا تتلقى تنبيهات للرسالة (لأن هذا هجوم محاكاة).

- التقارير: بعد اكتمال الهجوم المحاكاة، يمكنك النقر **فوق** تفاصيل الهجوم لرؤية التقرير.

- للحصول على إرشادات مفصلة وميزات جديدة في "محاكي الهجوم"، راجع [محاكي](/microsoft-365/security/office-365-security/attack-simulator)الهجوم في Microsoft 365 .
