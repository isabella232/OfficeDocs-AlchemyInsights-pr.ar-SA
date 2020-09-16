---
title: مشكله التنشيط-تعذر الاتصال حاليا
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725970"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>إصلاح تطبيقات Microsoft 365 "تعذر الاتصال الآن"

إذا تلقيت هذه الرسالة ، فجرب ما يلي:

1. تحقق من جدار الحماية وبرنامج مكافحه الفيروسات وإعدادات الوكيل للتاكد من انها لا تحظر الوصول إلى تطبيقات Microsoft 365 علي الإنترنت. راجع [نطاقات عناوين IP و url في Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. انتقل إلى **بدء**  >  **التشغيل**، ثم اكتب **services.msc**. تاكد من تشغيل كل الخدمات التالية:
    - اعداد تلقائي للاجهزه المتصلة بالشبكة
    - خدمه قائمه الشبكات
    - معرفه موقع الشبكة
    - سجل احداث Windows

إذا لم يتم تشغيل أحدي هذه الخدمات ، فحاول بدء تشغيلها. إذا كانت لديك مشكله في بدء تشغيل الخدمة ، فقم بتشغيل الأمر التالي بفتح موجه الأوامر باستخدام أذونات مرتفعه:

**/scannow sfc**

بعد انتهاء هذا الأمر ، أعد تشغيل الكمبيوتر.

للحصول علي معلومات مفصله ، راجع ["عذرا ، يتعذر علينا الاتصال بحسابك. يرجى المحاولة مره أخرى لاحقا "عند تنشيط Office من Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).