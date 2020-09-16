---
title: إصلاح تطبيقات Microsoft 365 تعذر العثور علي الرسالة المقترنة بتراخيص office
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747682"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>إصلاح الرسالة Microsoft 365 تعذر العثور علي تراخيص office المقترنة

إذا تلقيت هذه الرسالة ، فجرب ما يلي:

1. تحقق من جدار الحماية وبرنامج مكافحه الفيروسات وإعدادات الوكيل للتاكد من انها لا تحظر الوصول إلى تطبيقات Microsoft 365 علي الإنترنت. راجع [نطاقات عناوين IP و Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. أزاله [ترخيص Office وأعاده تعيينه](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) للمستخدم المتاثر. 
3. افتح تطبيق Office [وسجل خروجك](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) من اي حسابات مستخدمين موجودة.
4. انتقل إلى إعدادات Windows > البريد الكتروني **للحسابات**  >  **& الحسابات**، وقم بازاله كل حسابات العمل باستثناء الحساب المتاثر.
5. انتقل إلى إعدادات Windows > **الحسابات**  >  الخاصة**بالعمل أو المؤسسة التعليمية**، وقم بقطع اتصال كل حسابات العمل باستثناء الحساب المتاثر.
6. أعاده تعيين حاله تنشيط Office. [تعرف علي كيفيه القيام](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)بذلك.
7. [سجل الدخول](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) باستخدام حساب المستخدم المتاثر.

للحصول علي حلول اضافيه لاستكشاف الأخطاء وإصلاحها ، راجع [المنتج غير المرخص وأخطاء التنشيط في Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).