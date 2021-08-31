---
title: مشاكل في تسجيل الدخول Microsoft 365 التطبيقات
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
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744618"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>مشاكل في تسجيل الدخول Microsoft 365 Apps

ملاحظة: إذا كنت تستخدم إصدارا قديما من Windows (على سبيل المثال، Windows 7 SP1، Windows Server 2008 R2)، فاستخدم الإصلاح السهل لتمكين TLS 1.2 كافتراضي. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) لمزيد من المعلومات، راجع التحديث لتمكين [TLS 1.1 و TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)كبروتوكولات آمنة افتراضية في WinHTTP في Windows .

لإصلاح مشاكل تسجيل الدخول Microsoft 365 التطبيقات، جرب الخيارات التالية على الجهاز المتأثر:  

- للحصول Windows، راجع التوصيات حل مشاكل [تسجيل الدخول الشائعة](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- بالنسبة ل Mac، راجع [لا يمكن تسجيل الدخول إلى تطبيق Office 2016 for Mac Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**تلميح** على Windows الأجهزة، يمكننا تشخيص العديد من المشاكل الشائعة Office تسجيل الدخول وإصلاحها تلقائيا. قم بتنزيل **[Microsoft مساعد الإصلاح والدعم](https://aka.ms/SaRA-OfficeSignInScenario)** لاستخدام الأداة التلقائية.

**ملاحظة:** لا نوصي بتعطيل المصادقة الحديثة (ADAL) أو إدارة حساب ويب (WAM) لإصلاح مشاكل تسجيل الدخول أو **التنشيط.** إذا وقعت الأخطاء أثناء الاتصال Microsoft 365 باستخدام Office 2013، فتأكد [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) من تمكين المصادقة الحديثة Office العميل.

للحصول على إجراءات استكشاف الأخطاء وإصلاحها المحددة، راجع:

[مشاكل الاتصال في تسجيل الدخول بعد التحديث إلى Office 2016 16.0.7967 على Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[لا يمكنك تسجيل الدخول إلى حساب المؤسسة الخاص بك مثل Office 365 أو Azure أو Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[كيفية استكشاف الأخطاء وإصلاحها في التطبيقات غير المستعرضة التي لا يمكنها تسجيل الدخول إلى Office 365 أو Azure أو Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[المطالبة بشكل متكرر للحصول على بيانات الاعتماد في Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)