---
title: إصلاح تطبيقات Office عذرا، نحن تواجه رسالة مشكلات خادم مؤقت
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
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764104"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>إصلاح تطبيقات Office "عذراً، نحن نواجه مشاكل مؤقتة في الخادم"

إذا تلقيت هذه الرسالة، فجرّب ما يلي:

1. تحقق من جدار الحماية وبرامج مكافحة الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع الوصول إلى الإنترنت إلى تطبيقات Office. راجع [عناوين URL ونطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. انتقل إلى **بدء** > **تشغيل**، ثم اكتب **services.msc**. تأكد من تشغيل كافة الخدمات التالية:
    - الأجهزة المتصلة بالشبكة الإعداد التلقائي
    - خدمة قائمة الشبكة
    - التوعية بموقع الشبكة
    - سجل أحداث Windows

إذا لم يتم تشغيل إحدى هذه الخدمات، حاول بدء تشغيلها. إذا كان لديك مشكلة في بدء تشغيل الخدمة، قم بتشغيل الأمر التالي عن طريق فتح موجه أمر بأذونات مرتفعة:

**sfc / scannow**

بعد انتهاء هذا الأمر، أعد تشغيل الكمبيوتر.

للحصول على معلومات تفصيلية، راجع ["آسف، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مرة أخرى لاحقاً" خطأ عند تنشيط](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).