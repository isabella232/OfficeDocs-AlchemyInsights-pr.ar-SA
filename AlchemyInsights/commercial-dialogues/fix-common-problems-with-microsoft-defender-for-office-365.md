---
title: إصلاح المشاكل الشائعة في Microsoft Defender Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330047"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>إصلاح المشاكل الشائعة في Microsoft Defender Office 365

فيما يلي بعض الحلول للمشاكل الشائعة مع Microsoft Defender Office 365:

- **تأخير الرسالة**:

  قد يكون سبب التأخير في تسليم البريد الإلكتروني خزينة فحص المرفقات للرسائل. لمزيد من المعلومات، [راجع خزينة نهج المرفقات](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings).

- **الإبلاغ عن نتائج إيجابية أو سلبية خاطئة:**

  لمزيد من المعلومات، راجع [الإبلاغ عن الرسائل والملفات إلى Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **تمكين خزينة الارتباط:**

  1. في مدخل Microsoft 365 Defender، انتقل إلى البريد الإلكتروني & سياسات التعاون & قواعد خزينة الارتباطات في <https://security.microsoft.com/>  \>  \>  \>  **القسم** "سياسات".

     الانتقال مباشرة إلى صفحة ارتباطات **خزينة،** استخدم <https://security.microsoft.com/safelinksv2> .

  2. في صفحة **خزينة الارتباطات،** حدد النهج بالنقر فوق اسم النهج.
  3. في منتحل التفاصيل الذي يظهر، يمكنك القيام بأي من الخطوات التالية:
     - لإضافة نهج جديد، حدد **+ إنشاء**. سيتم تشغيل معالج لمساعدتك على تعريف إعدادات النهج.
     - لتحرير نهج موجود، حدد النهج بالنقر فوق اسم النهج. في قائمة التفاصيل التي تظهر، حدد **تحرير** في المقطع **إعدادات** الحماية.
  4. في الصفحة **إعدادات الحماية،** قم بتكوين الإعدادات التالية:
     - تشغيل تحديد **الإجراء لمعلومات URL** غير معروفة من المحتمل أن تكون ضارة في الرسائل .
     - حدد **تطبيق ارتباطات آمنة على الرسائل المرسلة داخل المؤسسة**.

  لمزيد من المعلومات، راجع إعداد [خزينة الارتباطات في Microsoft Defender Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies).
