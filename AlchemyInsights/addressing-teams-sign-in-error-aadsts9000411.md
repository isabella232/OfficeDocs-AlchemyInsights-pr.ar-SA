---
title: معالجة فرق تسجيل الدخول خطأ AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357259"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>معالجة فرق تسجيل الدخول خطأ AADSTS9000411

عند تسجيل الدخول إلى Microsoft Teams، قد تتلقى الخطأ: **عذراً، ولكن نا جناً مشكلة في تسجيل الدخول في AADSTS9000411: لم يتم تنسيق الطلب بشكل صحيح. يتم تكرار المعلمة "login_hint".**

لمعالجة هذه المشكلة، الرجاء التأكد من تحديث عملاء Microsoft Teams. لمزيد من المعلومات حول تحديث عميلك، راجع [تحديث فرق Microsoft](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

إذا لم تتمكن من تحديث العميل لسبب ما، سيؤدي تسجيل الخروج من العميل إلى مسح معظم البيانات المخزنة مؤقتًا. ومع ذلك، إذا كان لا يزال لديك مشاكل بعد تسجيل الخروج/تسجيل الدخول، إنهاء فرق الرجاء مسح ذاكرة التخزين المؤقت العميل الخاص بك عن طريق القيام بما يلي:
1. إغلاق فرق Microsoft.
2. انتقل إلى: %appdata%\microsoft\teams وحذف كافة الملفات.
3. إعادة فتح فرق Microsoft.
