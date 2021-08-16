---
title: BlockLegacyAuth
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
- "3154"
- "9001194"
ms.openlocfilehash: c2f2a0c3888920a969a6fc70af7ef7bfd8435bdcf975e0f31452b5da85e3a208
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968868"
---
# <a name="blocking-legacy-authentication"></a>حظر المصادقة القديمة

المصادقة القديمة عبارة عن مصطلح يشير إلى طلب مصادقة تم تقديمه من خلال:

- العملاء Office الذين لا يستخدمون المصادقة الحديثة (على سبيل المثال، Office 2010).

- أي عميل يستخدم بروتوكولات البريد القديمة مثل IMAP/SMTP/POP3.

لمزيد من المعلومات حول حظر المصادقة القديمة وتمكين المصادقة الحديثة، راجع [حظر المصادقة القديمة](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).

تجعل إعدادات الأمان الافتراضية في Azure Active Directory (Azure AD) من السهل أن تكون آمنا وتساعد على حماية مؤسستك. تحتوي إعدادات الأمان الافتراضية على إعدادات أمان تم تكوينها مسبقا للهجمات الشائعة.
لمزيد من المعلومات حول إعدادات الأمان الافتراضية، راجع [ما هي إعدادات الأمان الافتراضية؟](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults). 

**ملاحظة:** إذا تم إنشاء المستأجر في 22 أكتوبر 2019 أو بعده، فمن المحتمل أنك تواجه سلوك الأمان الافتراضي الجديد وقد تم تمكين إعدادات الأمان الافتراضية بالفعل في المستأجر.  في محاولة لحماية جميع المستخدمين، يتم طرح إعدادات الأمان الافتراضية لجميع المستأجرين الجدد الذين تم إنشاؤهم.
