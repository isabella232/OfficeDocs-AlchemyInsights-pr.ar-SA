---
title: إصلاح تطبيقات Microsoft 365 لا يمكن العثور على الرسالة المقترنة بتراخيص Office
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816475"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>إصلاح الرسالة "لم تتمكن من العثور على تراخيص Office المقترنة" في تطبيقات Microsoft 365

إذا تلقيت هذه الرسالة، فجرب ما يلي:

1. تحقق من جدار الحماية وبرامج الحماية من الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع الوصول إلى الإنترنت إلى تطبيقات Microsoft 365. راجع [عناوين URL 365 في Microsoft 365 نطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. قم [بإزالة ترخيص Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) للمستخدم المتأثر ثم إعادة تعيينه. 
3. افتح تطبيق Office و [سجل الخروج](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) من أي حسابات مستخدمين موجودة.
4. انتقل إلى إعدادات Windows > **حسابات** البريد الإلكتروني & الحسابات ، وأزل كل حسابات العمل باستثناء  >  الحساب المتأثر.
5. انتقل إلى إعدادات Windows > **حسابات** Access للعمل أو المدرسة ، واقطع اتصال كل حسابات العمل  >  باستثناء الحساب المتأثر.
6. إعادة تعيين حالة تنشيط Office. [تعرف على كيفية](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [سجل الدخول](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) باستخدام حساب المستخدم المتأثر.

للحصول على حلول إضافية حول استكشاف الأخطاء وإصلاحها، راجع أخطاء التنشيط والمنتج غير مرخص [في Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).