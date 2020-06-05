---
title: إصلاح تطبيقات Microsoft 365 عذرا، نحن تواجه رسالة مشاكل الخادم المؤقت
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582690"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>إصلاح تطبيقات Microsoft 365 "عذراً، نحن نواجه مشاكل مؤقتة في الخادم"

إذا تلقيت هذه الرسالة، فجرّب ما يلي:

1. تحقق من جدار الحماية وبرامج مكافحة الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع الوصول إلى الإنترنت إلى تطبيقات Microsoft 365. راجع [عناوين URL ونطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. انتقل إلى **بدء**  >  **تشغيل**، ثم اكتب **services.msc**. تأكد من تشغيل كافة الخدمات التالية:
    - الأجهزة المتصلة بالشبكة الإعداد التلقائي
    - خدمة قائمة الشبكة
    - التوعية بموقع الشبكة
    - سجل أحداث Windows

إذا لم يتم تشغيل إحدى هذه الخدمات، حاول بدء تشغيلها. إذا كان لديك مشكلة في بدء تشغيل الخدمة، قم بتشغيل الأمر التالي عن طريق فتح موجه أمر بأذونات مرتفعة:

**sfc / scannow**

بعد انتهاء هذا الأمر، أعد تشغيل الكمبيوتر.

للحصول على معلومات تفصيلية، راجع ["آسف، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مرة أخرى لاحقاً" خطأ عند تنشيط](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).