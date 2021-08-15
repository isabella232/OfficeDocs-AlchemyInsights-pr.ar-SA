---
title: ترحيل البريد الإلكتروني من خلال Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: ef06cfe41eee5d67bf82d4f64875ddafac82ee2062aade761f81b906cd428dd5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024193"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>إعداد جهاز أو تطبيق متعدد الوظائف لإرسال البريد الإلكتروني

للتعرّف على الخيارات والخطوات التي لديك، راجع [كيفية إعداد أي جهاز أو تطبيق متعدد الوظائف لإرسال البريد الإلكتروني باستخدام Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
إذا كان لديك جهاز أو تطبيق توقف عن العمل مؤخرا، فإن المشاكل الأكثر شيوعا هي:

- **الأخطاء المتعلقة بالمصادقة أثناء استخدام إرسال عميل SMTP Auth** لقد قمنا مؤخرا بإجراء بعض التغييرات المتعلقة بكيفية عمل مصادقة SMTP. لمزيد من المعلومات حول كيفية حل المشاكل، راجع قسم المصادقة غير الناجح في إصلاح المشاكل المتعلقة بالطابعات والماسحات الضوئية وتطبيقات LOB التي ترسل البريد الإلكتروني باستخدام Microsoft 365 [أو Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).
- **نحن نقبل إصدار TLS 1.2 فقط مع** إجراء اتصال آمن Office 365 إذا كنت تستخدم اتصال آمن (TLS)، فتأكد من أن جهاز التطبيق يدعم TLS 1.2. لمزيد من المعلومات، راجع التحضير ل [TLS 1.2 في](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)Office 365 Office 365 سحابة القطاع الحكومي .
 
للحصول على حلول وحلول أخرى، راجع إصلاح المشاكل المتعلقة [بالطابعات](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)والماسحات الضوئية وتطبيقات LOB التي ترسل البريد الإلكتروني باستخدام Microsoft 365 أو Office 365 .

للاطلاع على الأجهزة المتأثرة، انتقل إلى [تقرير عملاء مصادقة SMTP](https://protection.office.com/mailflow/dashboard).

**ملاحظة:** Exchange Online لا تتلاءم مع سيناريوهات البريد المجمع. لإرسال بريد إلكتروني تجاري مجمع (على سبيل المثال، رسائل العملاء الإخبارية)، يجب استخدام موفرين من جهة خارجية متخصصين في هذه الخدمات.
