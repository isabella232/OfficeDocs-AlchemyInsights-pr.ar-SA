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
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798667"
---
# <a name="unable-to-activate-office"></a>يتعذر تنشيط Office

**ملاحظة:** إذا كنت تستخدم إصدارا قديما من Windows (على سبيل المثال، Windows 7)، فتأكد من تمكين TLS 1.2 كافتراضي. لمزيد من المعلومات، راجع التحديث لتمكين [TLS 1.1 و TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)كبروتوكولات آمنة افتراضية في WinHTTP في Windows .

- تحقق مما إذا كانت حالة الاشتراك منتهية الصلاحية.
- تأكد من أن لديك اشتراكا يسمح بتراخيص العميل، مثل Office 365 Business أو ترخيص Premium، وتأكد من تعيين [ترخيص للمستخدم.](/microsoft-365/admin/manage/assign-licenses-to-users)
- تأكد من أن المستخدم يقوم بتسجيل الدخول إلى Office باستخدام الحساب نفسه الذي تم تعيين ترخيص له.
- تحقق من [صفحه حماية خدمة Office 365](/office365/enterprise/view-service-health) لمعرفه ما إذا كانت هناك أي مشكلات معروفة في الخدمة.
- تحقق من جدار الحماية وبرامج الحماية من الفيروسات وإعدادات الوكيل للتأكد من أنها لا تمنع Microsoft 365 الوصول إلى الإنترنت. الرجاء الاطلاع على [نطاقات عناوين IP وعناوين URL في Office 365](/office365/enterprise/urls-and-ip-address-ranges "نطاقات عناوين IP وعناوين URL في Office 365").

**تلميح** على Windows الأجهزة، يمكننا تشخيص العديد من مشاكل تسجيل الدخول الشائعة Office تلقائيا. قم بتنزيل **[Microsoft مساعد الإصلاح والدعم](https://aka.ms/SaRA-OfficeSignInScenario)** لاستخدام الأداة التلقائية.

استخدم إجراءات استكشاف الأخطاء وإصلاحها التالية:

- افتح أحد تطبيقات Office، ثم [قم بتسجيل الخروج](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)من أي حسابات مستخدم حالية. [قم بإزالة](/microsoft-365/admin/manage/remove-licenses-from-users) و[إعادة تعيين](/microsoft-365/admin/manage/assign-licenses-to-users) ترخيص Office، ثم [سجّل الدخول إلى Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) باستخدام حساب المستخدم المتأثر.
- تشغيل ["مستكشف أخطاء التنشيط ومصلحها"](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [إعادة تعيين حالة تنشيط Office](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "إعادة Office التنشيط")
- [قم بإجراء إصلاح Office عبر الإنترنت](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

للحصول على حلول إضافية لاستكشاف الأخطاء وإصلاحها، اطلع على:  

- [المنتج غير المرخص وأخطاء التنشيط في Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- ["عذراً، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مرة أخرى في وقت لاحق " خطأ يحدث عند تنشيط Office](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)