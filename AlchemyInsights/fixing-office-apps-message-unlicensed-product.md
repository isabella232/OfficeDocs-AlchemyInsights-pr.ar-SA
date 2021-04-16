---
title: تعذر تنشيط Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812559"
---
# <a name="unable-to-activate-office"></a>تعذر تنشيط Office

- تحقق مما إذا كانت حالة الاشتراك منتهية الصلاحية.
- تأكد من أن لديك اشتراكا يسمح بتراخيص العميل، مثل Office 365 Business أو Business Premium، وتأكد من تعيين [ترخيص للمستخدم](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).
- تأكد من أن المستخدم يقوم بتسجيل الدخول إلى Office باستخدام الحساب نفسه الذي تم تعيين ترخيص له.
- تحقق من [صفحه حماية خدمة Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) لمعرفه ما إذا كانت هناك أي مشكلات معروفة في الخدمة.
- تحقق من جدار الحماية وبرامج الحماية من الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع وصول تطبيقات Microsoft 365 إلى الإنترنت. الرجاء الاطلاع على [نطاقات عناوين IP وعناوين URL في Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "نطاقات عناوين IP وعناوين URL في Office 365").

**تلميح** على أجهزة Windows، يمكننا تشخيص العديد من مشاكل تسجيل الدخول الشائعة في Office وإصلاحها تلقائيا من أجلك. قم  **[بتنزيل مساعد الاسترداد والدعم من Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** وتشغيله لاستخدام الأداة التلقائية.

استخدم إجراءات استكشاف الأخطاء وإصلاحها التالية:

- افتح أحد تطبيقات Office، ثم [قم بتسجيل الخروج](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)من أي حسابات مستخدم حالية. [قم بإزالة](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) و[إعادة تعيين](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ترخيص Office، ثم [سجّل الدخول إلى Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) باستخدام حساب المستخدم المتأثر.
- تشغيل ["مستكشف أخطاء التنشيط ومصلحها"](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [إعادة تعيين حالة تنشيط Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "إعادة تعيين حالة تنشيط Office")
- [قم بإجراء إصلاح Office عبر الإنترنت](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

للحصول على حلول إضافية لاستكشاف الأخطاء وإصلاحها، اطلع على:  

- [المنتج غير المرخص وأخطاء التنشيط في Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- ["عذراً، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مرة أخرى في وقت لاحق " خطأ يحدث عند تنشيط Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)