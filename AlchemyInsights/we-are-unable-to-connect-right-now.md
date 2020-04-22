---
title: مشكلة التنشيط - نحن غير قادرين على الاتصال الآن
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716159"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>إصلاح رسالة تطبيقات Office "نحن غير قادرين على الاتصال الآن"

إذا تلقيت هذه الرسالة، فجرّب ما يلي:

1. تحقق من جدار الحماية وبرامج مكافحة الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع الوصول إلى الإنترنت إلى تطبيقات Office. راجع [عناوين URL لـ Microsoft ونطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. انتقل إلى **بدء** > **تشغيل**، ثم اكتب **services.msc**. تأكد من تشغيل كافة الخدمات التالية:
    - الأجهزة المتصلة بالشبكة الإعداد التلقائي
    - خدمة قائمة الشبكة
    - التوعية بموقع الشبكة
    - سجل أحداث Windows

إذا لم يتم تشغيل إحدى هذه الخدمات، حاول بدء تشغيلها. إذا كان لديك مشكلة في بدء تشغيل الخدمة، قم بتشغيل الأمر التالي عن طريق فتح موجه أمر بأذونات مرتفعة:

**sfc / scannow**

بعد انتهاء هذا الأمر، أعد تشغيل الكمبيوتر.

للحصول على معلومات تفصيلية، راجع ["آسف، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مرة أخرى لاحقاً" خطأ عند تنشيط Office من Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).