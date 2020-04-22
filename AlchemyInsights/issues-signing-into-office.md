---
title: مشكلات تسجيل الدخول إلى تطبيقات Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762962"
---
# <a name="issues-signing-in-to-office-apps"></a>مشكلات تسجيل الدخول إلى تطبيقات Office

لإصلاح مشكلات تسجيل الدخول مع تطبيقات Office، جرّب ما يلي:

- قم بإزالة كافة حسابات العمل، باستثناء الحساب المتأثر، باستخدام إعدادات Windows > **الوصول إلى العمل أو المدرسة**.
- [مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.<br/>
    **ملاحظة:** تم تغيير مسارات التسجيل لـ Office 2016 إلى 16.0. (على سبيل: \Software\Microsoft\Office\16.0\Common\Identity\)
- افتح تطبيق Office، اختر**تسجيل الخروج****من حساب** >  **الملف** > . ثم قم بتسجيل الدخول باستخدام حساب مستخدم بترخيص صالح. للحصول على معلومات مفصلة، راجع [حسابات في Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- بالنسبة لأجهزة Mac، راجع [يتعذر عليك تسجيل الدخول إلى تطبيق Office 2016 for Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- إذا حدثت الأخطاء أثناء الاتصال بـ Microsoft 365 باستخدام Office 2013، قم بتمكين المصادقة الحديثة لعميل Office.

لمزيد من المعلومات، اطلع على:
- [لا يمكنك تسجيل الدخول إلى Microsoft 365 أو Azure أو Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [مشكلات الاتصال في تسجيل الدخول بعد التحديث إلى Office 2016 إنشاء 16.0.7967 على Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["عذراً، تم تسجيل الدخول بالفعل إلى حساب آخر من مؤسستك على هذا الكمبيوتر" في Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [استكشاف مشكلات تسجيل الدخول وإصلاحها باستخدام مصادقة Office الحديثة عند استخدام ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)