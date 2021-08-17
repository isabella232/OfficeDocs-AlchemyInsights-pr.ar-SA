---
title: 2491 تنبيه رسائل البريد الإلكتروني من نهج "تسليم التصيد الاحتيالي بسبب تجاوز المستأجر أو المستخدم"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e24f489292f38b5e9cacc8b9bfe5730ebfc71ce5e3004be479134ef6c791a12
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899319"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>تنبيه رسائل البريد الإلكتروني من نهج "تسليم التصيد الاحتيالي بسبب تجاوز المستأجر أو المستخدم"

يتوفر نهج تنبيه افتراضي يسمى **"تسليم** التصيد الاحتيالي" بسبب تجاوز المستأجر أو المستخدم في المؤسسات التي تستخدم Microsoft Defender Office 365 P1 و P2. إذا تلقيت هذا التنبيه، فيما يلي الخطوات اللازمة للتحقق من ذلك:

1. من رسالة التنبيه، انقر فوق **عرض** التنبيهات الانتقال إلى صفحة التنبيهات في Microsoft 365 Defender المدخل. 

2. حدد التنبيه لرؤية الخيار لعرض **قائمة** الرسائل أو **عرض الرسائل في المستكشف**. يأخذك كل من هذين الخيارين إلى تفاصيل الرسالة، التي تتضمن "معرّف الرسالة". تجدر الإشارة إلى أن الارتباط "مستكشف التهديدات" سيصفي الرسائل التي تتطابق مع معايير التنبيه تلقائيا. قد تحتاج إلى ضبط عامل تصفية التاريخ في "مستكشف التهديدات".

تم تسليم رسالة التصيد الاحتيالي بسبب تجاوز تم تكوينه يدويا:

- مرسل مسموح به أو مجال تم تعيينه بواسطة المستخدم.
- مرسل مسموح به أو مجال تم تعيينه من قبل المسؤول في نهج مكافحة البريد العشوائي.
- عنوان IP مسموح به في نهج عامل تصفية الاتصال.
- قاعدة تدفق البريد (المعروفة أيضا باسم قاعدة النقل) التي تم تكوينها للسماح بالرسائل الواردة.

إذا كنت تعتقد أنه تم وضع علامة تصيد احتيالي على الرسالة بشكل غير صحيح، فاستخدم إرسال [المسؤول](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) لتقديم تقرير بالرسالة إلى Microsoft.

يمكن للمستخدمين استخدام الوظائف الإضافية ["الإبلاغ](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) عن رسالة" أو الوظائف الإضافية "الإبلاغ عن التصيد الاحتيالي" Outlook لإرسال نماذج الرسائل إلى Microsoft.
