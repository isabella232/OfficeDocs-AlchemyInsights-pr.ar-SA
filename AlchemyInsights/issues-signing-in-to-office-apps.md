---
title: المشاكل المتعلقة بتسجيل الدخول إلى تطبيقات Microsoft 365
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
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695310"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>إصلاح تطبيقات Microsoft 365 "عذرا ، تم تسجيل دخول حساب آخر من مؤسستك بالفعل" في الرسالة

لإصلاح هذا الخطأ، حاول القيام بالخطوات التالية:

- قم بازاله كل حسابات العمل ، باستثناء الحساب المتاثر ، باستخدام إعدادات Windows > **الوصول إلى العمل أو المؤسسة التعليمية**.
- [مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام "أداره بيانات اعتماد Windows".<br/>
    **ملاحظه:** لقد تغيرت مسارات التسجيل ل Office 2016 إلى 16.0. (علي سبيل المثال: \Software\Microsoft\Office\16.0\Common\Identity\)
- افتح تطبيق Office ، واختر **File**  >  **Account**  >  **تسجيل الخروج**من حساب الملفات. ثم سجل دخولك باستخدام حساب مستخدم بترخيص صالح. للحصول على معلومات مفصلة، راجع [حسابات في Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- بالنسبة لأجهزة Mac، راجع [يتعذر عليك تسجيل الدخول إلى تطبيق Office 2016 for Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

لمزيد من المعلومات ، راجع ["معذره ، تم تسجيل دخول حساب آخر من مؤسستك بالفعل علي هذا الكمبيوتر" في Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).