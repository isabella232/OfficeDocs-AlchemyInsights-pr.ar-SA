---
title: مشكلة في AAD Connect Health
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480863"
---
# <a name="problem-with-aad-connect-health"></a>مشكلة في حالة اتصال AAD

- تأكد من أنك مفوض لتنفيذ العملية. يمكن للمسؤولين العامين الوصول بشكل افتراضي. بالإضافة إلى ذلك، يمكنك استخدام "التحكم بالوصول المستند [إلى الدور"](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) لتفويض إذن التسجيل للمساهم.
- تأكد من تمكين نقاط النهاية المطلوبة، ومن عدم حظرها بسبب جدار الحماية. للحصول على التفاصيل، راجع [المتطلبات.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- قد يفشل التسجيل بسبب خضع الاتصال الصادر لفحص SSL بواسطة طبقة الشبكة.
- تأكد من أنك قمت بالتحقق من إعدادات الإعلامات الخاصة ب Azure AD Connect Health. يرجى مراجعة الإعداد. يمكن [أن](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) يساعدك هذا الدليل على فهم كيفية تكوين إعدادات الإعلامات لإعلامات Azure AD Connect الصحية.
- لمعرفة المزيد حول تقرير مزامنة AAD Connect Health وكيفية تنزيله، راجع تقرير [مزامنة مستوى الكائن.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

استكشاف الأخطاء في تنبيهات AAD Connect Health وإصلاحها، اتبع دليل استكشاف الأخطاء وإصلاحها لتنبيهات سطوع بيانات [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) والأسئلة الشائعة، راجع أسئلة تثبيت [Common AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
