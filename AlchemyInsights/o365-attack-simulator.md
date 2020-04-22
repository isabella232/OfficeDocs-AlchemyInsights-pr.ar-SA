---
title: 2681 هجوم محاكي في مايكروسوفت 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713453"
---
# <a name="attack-simulator-in-microsoft-365"></a>محاكاة الهجوم في مايكروسوفت 365

- هل تفتقد محاكي الهجوم؟ يتطلب محاكي الهجوم **Office 365 خطة متقدمة للحماية من التهديدات 2 (خطة ATP 2)** أو **Office 365 Enterprise E5**. **لا** يتم تضمين محاكي الهجوم في Office 365 خطة الحماية المتقدمة من التهديدات 1 (خطة ATP 1) أو Office 365 Enterprise E3 أو أي تطبيقات Microsoft 365 لاشتراكات الأعمال.

- يتطلب الحساب الذي تستخدمه لإطلاق هجمات محاكاة أذونات المسؤول أو مسؤول الأمان العمومية والمصادقة متعددة العوامل (MFA). لمزيد من المعلومات حول متطلبات محاكي الهجوم، راجع [هذا الموضوع](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- أشياء هامة لمعرفة عن محاكاة هجوم **كلمة مرور القوة الغاشمة:**

  - إذا تم تمكين حساب الهدف MFA وتم تخمين كلمة المرور بشكل صحيح، فلن يظهر الحساب كما تم اختراقه (سيكون عامل المصادقة الثاني غير مكتمل).

  - لا يمكن أن يكون ملف كلمة المرور أكبر من 10 ميغابايت. استخدم كلمة مرور واحدة لكل سطر، وتضمين سطر فارغ (إرجاع النقل) بعد كلمة المرور الأخيرة في القائمة.

- أشياء هامة يجب معرفتها عن محاكاة **ربط التصيد الاحتيالي بالرمح:**

  - حسب التصميم، لا يمكنك توفير قيمة مخصصة **لعنوان URL لخادم تسجيل الدخول التصيدي**.

  - إذا استخدم المستلم [الوظيفة الإضافية تمكين رسالة التقرير](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) للإبلاغ عن الرسالة كخداع، فقد لا تتلقى تنبيهات للرسالة (لأن هذا هجوم محاكاة).

- التقارير: بعد اكتمال الهجوم المحاكي، يمكنك النقر فوق **تفاصيل الهجوم** لمشاهدة التقرير.

- للحصول على إرشادات مفصلة وميزات جديدة في محاكي الهجوم، راجع [محاكي الهجوم في Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
