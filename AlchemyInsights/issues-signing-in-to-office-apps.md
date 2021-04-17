---
title: مشاكل في تسجيل الدخول إلى تطبيقات Microsoft 365
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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833062"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>تصحيح رسالة تطبيقات Microsoft 365 "عذرا، حساب آخر من مؤسستك قد تم بالفعل الدخول"

لإصلاح هذا الخطأ، حاول القيام بالخطوات التالية:

- قم بإزالة كل حسابات العمل، باستثناء الحساب المتأثر، باستخدام إعدادات Windows > **Access للعمل أو المدرسة.**
- [مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.<br/>
    **ملاحظة:** تم تغيير مسارات التسجيل ل Office 2016 إلى 16.0. (على ما يلي: \Software\Microsoft\Office\16.0\Common\Identity\)
- افتح تطبيق Office، واختر **تسجيل**  >  **الخروج من** حساب  >  **الملف**. ثم سجل الدخول باستخدام حساب مستخدم مع ترخيص صالح. للحصول على معلومات مفصلة، راجع [حسابات في Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- بالنسبة لأجهزة Mac، راجع [يتعذر عليك تسجيل الدخول إلى تطبيق Office 2016 for Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

لمزيد من المعلومات، راجع ["عذرا، حساب](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)آخر من مؤسستك قد تم بالفعل في هذا الكمبيوتر" في Office .