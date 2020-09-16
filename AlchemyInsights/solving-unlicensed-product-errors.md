---
title: حل أخطاء المنتج غير المرخص
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
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737940"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>اقتراحات لحل الأخطاء "منتج غير مرخص"

لحل الأخطاء المتعلقة بمنتج غير مرخص ، جرب ما يلي:

- تحقق لمعرفه ما إذا كانت حاله الاشتراك قد انتهت صلاحيتها.
- تاكد من ان لديك اشتراك يسمح لتراخيص العميل ، مثل تطبيقات Microsoft 365 للاعمال أو الشركات المتميزة ، [وتاكد من ان المستخدم يملك ترخيصا معينا](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- تاكد من ان المستخدم سيقوم بتسجيل الدخول إلى Office باستخدام الحساب نفسه الذي تم تعيين الترخيص له.
- تحقق من [صفحه حماية الخدمة](https://docs.microsoft.com/office365/enterprise/view-service-health) لمعرفه ما إذا كانت هناك اي مشاكل معروفه تتعلق بالخدمة.
- تحقق من جدار الحماية وبرنامج مكافحه الفيروسات وإعدادات الوكيل للتاكد من انها لا تحظر وصول تطبيقات Microsoft 365 إلى الإنترنت. راجع [نطاقات عناوين IP و url](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

قد تجرب أيضا إجراءات استكشاف الأخطاء وإصلاحها التالية: 

- افتح تطبيق Office [وسجل خروجك](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) من اي حسابات مستخدمين موجودة. قم [بازاله](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) ترخيص office [وأعاده تعيينه](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ، ثم قم [بتسجيل الدخول إلى Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) باستخدام حساب المستخدم المتاثر.
- شغل [مستكشف أخطاء التنشيط ومصلحها](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [أعاده تعيين حاله تنشيط Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [قم باجراء إصلاح عبر الإنترنت ل Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

للحصول على حلول إضافية لاستكشاف الأخطاء وإصلاحها، اطلع على: 

- [المنتج غير المرخص وأخطاء التنشيط في Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- ["عذراً، لا يمكننا الاتصال بحسابك. الرجاء المحاولة مرة أخرى في وقت لاحق " خطأ يحدث عند تنشيط Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)