---
title: مشكلات تسجيل الدخول إلى تطبيقات Microsoft 365
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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579924"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>إصلاح تطبيقات Microsoft 365 "عذراً، تم تسجيل الدخول بالفعل لحساب آخر من مؤسستك"

لإصلاح هذا الخطأ، حاول القيام بالخطوات التالية:

- قم بإزالة كافة حسابات العمل، باستثناء الحساب المتأثر، باستخدام إعدادات Windows > **الوصول إلى العمل أو المدرسة**.
- [مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.<br/>
    **ملاحظة:** تم تغيير مسارات التسجيل لـ Office 2016 إلى 16.0. (على سبيل: \Software\Microsoft\Office\16.0\Common\Identity\)
- افتح تطبيق Office، اختر تسجيل الخروج من حساب **الملف**  >  **Account**  >  **Sign Out**. ثم قم بتسجيل الدخول باستخدام حساب مستخدم بترخيص صالح. للحصول على معلومات مفصلة، راجع [حسابات في Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- بالنسبة لأجهزة Mac، راجع [يتعذر عليك تسجيل الدخول إلى تطبيق Office 2016 for Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

لمزيد من المعلومات، راجع ["عذراً، تم تسجيل الدخول بالفعل لحساب آخر من مؤسستك على هذا الكمبيوتر" في Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).