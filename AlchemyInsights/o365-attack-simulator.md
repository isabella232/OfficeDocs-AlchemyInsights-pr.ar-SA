---
title: محاكي الهجوم في 2681 في Microsoft 365
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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801530"
---
# <a name="attack-simulator-in-microsoft-365"></a>محاكي الهجوم في Microsoft 365

- هل أنت تفتقد إلى محاكي الهجوم ؟ يتطلب محاكي **الهجوم توفر Microsoft Defender ل Office 365 الخطة 2 (خطه ATP 2)** أو **Office 365 Enterprise E5** . **لم** يتم تضمين محاكي الهجوم في Microsoft Defender ل Office 365 الخطة 1 (خطه ATP 1) أو Office 365 Enterprise E3 أو اي تطبيقات Microsoft 365 للاشتراكات التجارية.

- يتطلب الحساب الذي تستخدمه لبدء الهجمات المحاكية أذونات المسؤول العام أو مسؤول الأمان ومصادقه متعددة العوامل (MFA). لمزيد من المعلومات حول متطلبات محاكي الهجوم ، راجع [هذا الموضوع](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- الأمور الهامه التي يجب معرفتها حول عمليات محاكاة هجوم **كلمه المرور برتي**

  - إذا كان الحساب الهدف تم تمكين MFA عليه وكانت كلمه المرور جسده بشكل صحيح ، فلن يظهر الحساب كتم اختراقه (سيكتمل عامل المصادقة الثاني).

  - لا يمكن ان يكون ملف كلمه المرور أكبر من 10 ميغابايت. استخدم كلمه مرور واحده لكل سطر ، وقم بتضمين سطر فارغ (حرف إرجاع) بعد كلمه المرور الاخيره في القائمة.

- الأمور الهامه التي يجب معرفتها حول عمليات محاكاة **الشبير في التصيد الاحتيالي** :

  - بحسب التصميم ، لا يمكنك توفير قيمه مخصصه **لعنوان URL لخادم تسجيل الدخول إلى التصيد الاحتيالي** .

  - إذا كان أحد المستلمين يستخدم [الوظيفة الاضافيه الخاصة برسائل التقرير](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) للإبلاغ عن الرسالة كتصيد احتيالي ، فقد لا تتلقي تنبيات للرسالة (لان هذا الهجوم تمت محاكاته).

- التقارير: بعد اكتمال الهجوم الذي تمت محاكاته ، يمكنك النقر فوق **تفاصيل الهجوم** لعرض التقرير.

- للحصول علي الإرشادات التفصيلية والميزات الجديدة في محاكي الهجوم ، راجع [محاكي الهجوم في Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
