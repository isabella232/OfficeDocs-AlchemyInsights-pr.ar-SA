---
title: إصلاح تطبيقات Microsoft 365 عذرا ، نواجه رسالة مشاكل مؤقته في الخادم
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758232"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>إصلاح تطبيقات Microsoft 365 "عذرا ، فنحن نواجه مشكلات مؤقته في الخادم"

إذا تلقيت هذه الرسالة ، فجرب ما يلي:

1. تحقق من جدار الحماية وبرنامج مكافحه الفيروسات وإعدادات الوكيل للتاكد من انها لا تحظر الوصول إلى تطبيقات Microsoft 365 علي الإنترنت. راجع [نطاقات عناوين IP و url](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. انتقل إلى **بدء**  >  **التشغيل**، ثم اكتب **services.msc**. تاكد من تشغيل كل الخدمات التالية:
    - اعداد تلقائي للاجهزه المتصلة بالشبكة
    - خدمه قائمه الشبكات
    - معرفه موقع الشبكة
    - سجل احداث Windows

إذا لم يتم تشغيل أحدي هذه الخدمات ، فحاول بدء تشغيلها. إذا كانت لديك مشكله في بدء تشغيل الخدمة ، فقم بتشغيل الأمر التالي بفتح موجه الأوامر باستخدام أذونات مرتفعه:

**/scannow sfc**

بعد انتهاء هذا الأمر ، أعد تشغيل الكمبيوتر.

للحصول علي معلومات مفصله ، راجع ["عذرا ، يتعذر علينا الاتصال بحسابك. الرجاء المحاولة مره أخرى لاحقا "عند التنشيط](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).