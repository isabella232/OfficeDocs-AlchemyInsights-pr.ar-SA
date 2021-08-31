---
title: تصحيح Microsoft 365 عذرا، لدينا رسالة مشاكل مؤقتة في الخادم
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
- "3420"
- "9001430"
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744620"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>تصحيح رسالة Microsoft 365 "عذرا، نحن نواجه مشاكل مؤقتة في الخادم"

ملاحظة: إذا كنت تستخدم إصدارا قديما من Windows (على سبيل المثال، Windows 7 SP1، Windows Server 2008 R2)، فاستخدم الإصلاح السهل لتمكين TLS 1.2 كافتراضي. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) لمزيد من المعلومات، راجع التحديث لتمكين [TLS 1.1 و TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)كبروتوكولات آمنة افتراضية في WinHTTP في Windows .

إذا تلقيت هذه الرسالة، فجرب ما يلي:

1. تحقق من جدار الحماية وبرامج الحماية من الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع الوصول إلى الإنترنت Microsoft 365 التطبيقات. راجع [عناوين URL ونطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. انتقل إلى **بدء**  >  **تشغيل**، ثم اكتب **services.msc**. تأكد من تشغيل الخدمات التالية كلها:
    - الإعداد التلقائي للأجهزة المتصلة بالشبكة
    - خدمة قائمة الشبكة
    - الوعي بموقع الشبكة
    - Windows سجل الأحداث

إذا لم تكن إحدى هذه الخدمات قيد التشغيل، فحاول بدء تشغيلها. إذا كانت لديك مشكلة في بدء تشغيل الخدمة، فدير الأمر التالي بفتح موجه أوامر بأذونات مرتفعة:

**sfc /scannow**

بعد انتهاء هذا الأمر، أعد تشغيل الكمبيوتر.

للحصول على معلومات مفصلة، راجع ["عذرا، لا يمكننا الاتصال حسابك. يرجى المحاولة مرة أخرى لاحقا" عند تنشيط](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).