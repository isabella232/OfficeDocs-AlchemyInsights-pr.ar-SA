---
title: إصلاح تطبيقات Microsoft 365 حسابك في رسالة حاله سيئه
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744532"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>إصلاح تطبيقات Microsoft 365 "حسابك في حاله سيئه"

لإصلاح هذا الخطا ، جرب الخيارات التالية علي الكمبيوتر المتاثر:

- افتح تطبيق Office ، وحدد **File**  >  **حساب**  >  **الملفات الخاصة بكل الحسابات**. سجل الدخول مره أخرى باستخدام حساب مستخدم مع ترخيص صالح. للحصول على معلومات مفصلة، راجع [حسابات في Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام "أداره بيانات اعتماد Windows".<br>
  **ملاحظه:** لقد تغيرت مسارات التسجيل ل Office 2016 إلى 16.0. علي سبيل المثال ، \Software\Microsoft\Office\16.0\Common\Identity\
- إذا حدث الخطا اثناء الاتصال ب Office 365 باستخدام Office 2013 ، فقم [بتمكين المصادقة الحديثة](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) لعميل Office.

لمزيد من المعلومات ، راجع [كيفيه استكشاف أخطاء التطبيقات غير التابعة للمستعرض التي لا يمكنها تسجيل الدخول إلى Microsoft 365 أو Azure أو Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

