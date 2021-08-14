---
title: مشكلة في AAD الاتصال الصحة
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
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923739"
---
# <a name="problem-with-aad-connect-health"></a>مشكلة في AAD الاتصال الصحة

- تأكد من أنك م مخولا لتنفيذ العملية. يمكن للمسؤولين العامين الوصول بشكل افتراضي. بالإضافة إلى ذلك، يمكنك استخدام ["التحكم بالوصول المستند](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) إلى الدور" لتفويض إذن التسجيل إلى المساهم.
- تأكد من تمكين نقاط النهاية المطلوبة، ولا يتم حظرها بسبب جدار الحماية. للحصول على التفاصيل، راجع [المتطلبات](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- قد يفشل التسجيل بسبب تعرض الاتصال الصادر لفحص SSL بواسطة طبقة الشبكة.
- تأكد من التحقق من إعدادات الإعلامات ل Azure AD الاتصال Health. الرجاء مراجعة الإعداد. يمكن [أن](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) يساعدك هذا الدليل على فهم كيفية تكوين إعدادات الإعلامات ل Azure AD الاتصال الإعلامات الصحية.
- لمعرفة المزيد حول تقرير مزامنة الاتصال AAD وكيفية تنزيله، راجع تقرير مزامنة [مستوى الكائن](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

لاستعلام تنبيهات AAD الاتصال Health وإصلاحها، اتبع دليل استكشاف الأخطاء وإصلاحها [لتنبيهات](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) نضار بيانات AAD الاتصال الصحية والأسئلة الشائعة، راجع الأسئلة الشائعة حول تثبيت [AAD الاتصال Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
