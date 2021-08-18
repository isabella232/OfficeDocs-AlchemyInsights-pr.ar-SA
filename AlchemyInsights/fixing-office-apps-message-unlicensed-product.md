---
title: يتعذر تنشيط Office
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
ms.openlocfilehash: a057aaa2ddf8885b96c0fe0d5fa87d3a1b191af9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327833"
---
# <a name="unable-to-activate-office"></a>يتعذر تنشيط Office

**ملاحظة:** إذا كنت تستخدم إصدارا قديما من Windows (على سبيل المثال، Windows 7)، فتأكد من تمكين TLS 1.2 كافتراضي. لمزيد من المعلومات، راجع التحديث لتمكين [TLS 1.1 و TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)كبروتوكولات آمنة افتراضية في WinHTTP في Windows .

- تحقق مما إذا كانت حالة الاشتراك منتهية الصلاحية.
- تأكد من أن لديك اشتراكا يسمح بتراخيص العميل، مثل Office 365 Business أو Business Premium، وتأكد من تعيين ترخيص [للمستخدم.](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)
- تأكد من أن المستخدم يقوم بتسجيل الدخول إلى Office باستخدام الحساب نفسه الذي تم تعيين ترخيص له.
- تحقق من [صفحه حماية خدمة Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) لمعرفه ما إذا كانت هناك أي مشكلات معروفة في الخدمة.
- تحقق من جدار الحماية وبرامج الحماية من الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع Microsoft 365 الوصول إلى الإنترنت. الرجاء الاطلاع على [نطاقات عناوين IP وعناوين URL في Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "نطاقات عناوين IP وعناوين URL في Office 365").

**تلميح** على Windows، يمكننا تشخيص العديد من مشاكل تسجيل الدخول الشائعة وإصلاحها تلقائيا Office تسجيل الدخول. قم بتنزيل **[Microsoft مساعد الإصلاح والدعم](https://aka.ms/SaRA-OfficeSignInScenario)** لاستخدام الأداة التلقائية.

استخدم إجراءات استكشاف الأخطاء وإصلاحها التالية:

- افتح أحد تطبيقات Office، ثم [قم بتسجيل الخروج](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)من أي حسابات مستخدم حالية. [قم بإزالة](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) و[إعادة تعيين](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ترخيص Office، ثم [سجّل الدخول إلى Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) باستخدام حساب المستخدم المتأثر.
- تشغيل ["مستكشف أخطاء التنشيط ومصلحها"](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [إعادة تعيين حالة تنشيط Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "إعادة Office التنشيط")
- [قم بإجراء إصلاح Office عبر الإنترنت](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

للحصول على حلول إضافية لاستكشاف الأخطاء وإصلاحها، اطلع على:  

- [المنتج غير المرخص وأخطاء التنشيط في Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- ["عذراً، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مرة أخرى في وقت لاحق " خطأ يحدث عند تنشيط Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)