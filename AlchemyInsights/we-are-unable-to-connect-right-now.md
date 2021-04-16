---
title: مشكلة التنشيط - يتعذر علينا الاتصال الآن
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
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806429"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>إصلاح رسالة تطبيقات Microsoft 365 "تعذر الاتصال الآن"

إذا تلقيت هذه الرسالة، فجرب ما يلي:

1. تحقق من جدار الحماية وبرامج الحماية من الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع الوصول إلى الإنترنت إلى تطبيقات Microsoft 365. راجع [عناوين URL ونطاقات عناوين IP ل Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. انتقل إلى **بدء**  >  **تشغيل**، ثم اكتب **services.msc**. تأكد من تشغيل جميع الخدمات التالية:
    - الإعداد التلقائي للأجهزة المتصلة بالشبكة
    - خدمة قائمة الشبكة
    - الوعي بموقع الشبكة
    - سجل أحداث Windows

إذا لم تكن إحدى هذه الخدمات قيد التشغيل، فحاول بدء تشغيلها. إذا كانت لديك مشكلة في بدء تشغيل الخدمة، فدير الأمر التالي بفتح موجه أوامر بأذونات مرتفعة:

**sfc /scannow**

بعد انتهاء هذا الأمر، أعد تشغيل الكمبيوتر.

للحصول على معلومات مفصلة، راجع ["عذرا، لا يمكننا الاتصال حسابك. يرجى المحاولة مرة أخرى لاحقا" عند تنشيط Office من Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).