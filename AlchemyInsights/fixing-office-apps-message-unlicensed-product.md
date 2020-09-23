---
title: تعذر تنشيط Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: e052c18eae035ff05c70a223f6d8a2eab875b2c9
ms.sourcegitcommit: 57102d7daf32f370cab84dba342819a1ad5cb261
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/23/2020
ms.locfileid: "48236076"
---
# <a name="unable-to-activate-office"></a>تعذر تنشيط Office

- تحقق مما إذا كانت حالة الاشتراك منتهية الصلاحية.
- تاكد من ان لديك اشتراك يسمح لتراخيص العميل ، مثل Office 365 Business أو Business Premium ، [وتاكد من ان المستخدم قد تم تعيين ترخيص له](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users).
- تأكد من أن المستخدم يقوم بتسجيل الدخول إلى Office باستخدام الحساب نفسه الذي تم تعيين ترخيص له.
- تحقق من [صفحه حماية خدمة Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) لمعرفه ما إذا كانت هناك أي مشكلات معروفة في الخدمة.
- التحقق من جدار الحماية وبرنامج الحماية من الفيروسات وإعدادات الوكيل للتاكد من انها لا تحظر وصول تطبيقات Microsoft 365 إلى الإنترنت. الرجاء الاطلاع على [نطاقات عناوين IP وعناوين URL في Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "نطاقات عناوين IP وعناوين URL في Office 365").

**تلميح** في أجهزه Windows ، يمكننا تشخيص العديد من المشاكل الشائعة في تسجيل الدخول إلى Office وإصلاحها بالنيابة عنك. يمكنك تنزيل  **[مساعد الإصلاح والدعم من Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** وتشغيله لاستخدام الاداه التلقائية الخاصة بنا.

استخدم إجراءات استكشاف الأخطاء وإصلاحها التالية:

- افتح أحد تطبيقات Office، ثم [قم بتسجيل الخروج](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)من أي حسابات مستخدم حالية. [قم بإزالة](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) و[إعادة تعيين](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ترخيص Office، ثم [سجّل الدخول إلى Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) باستخدام حساب المستخدم المتأثر.
- تشغيل ["مستكشف أخطاء التنشيط ومصلحها"](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [إعادة تعيين حالة تنشيط Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "أعاده تعيين حاله تنشيط Office")
- [قم بإجراء إصلاح Office عبر الإنترنت](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

للحصول على حلول إضافية لاستكشاف الأخطاء وإصلاحها، اطلع على:  

- [المنتج غير المرخص وأخطاء التنشيط في Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- ["عذراً، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مرة أخرى في وقت لاحق " خطأ يحدث عند تنشيط Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)