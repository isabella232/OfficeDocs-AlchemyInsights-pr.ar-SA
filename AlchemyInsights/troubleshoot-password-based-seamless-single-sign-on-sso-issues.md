---
title: استكشاف مشاكل تسجيل الدخول المفرد السلس (SSO) المستندة إلى كلمة المرور وإصلاحها
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
- "9004357"
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972811"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>استكشاف مشاكل تسجيل الدخول المفرد السلس (SSO) المستندة إلى كلمة المرور وإصلاحها

للتعرف على أساسيات SSO المستند إلى كلمة المرور، راجع المصادقة المستندة إلى كلمة المرور [باستخدام Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**تكوين SSO المستند إلى كلمة المرور**

1. [تكوين تسجيل الدخول](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) الفردي المستند إلى كلمة المرور - تدخل هذه المقالة في مزيد من التفاصيل حول خيار تسجيل الدخول الموحد المستند إلى كلمة المرور. إذا كان التطبيق الذي تقوم بإضافته يتطلب تكوينا مخصصا وتحتاج إلى استخدام SSO قائم على كلمة المرور، فهذا يعني أن هذه المقالة مخصصة لك.
2. [تكوين تسجيل الدخول الفردي المستند](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) إلى كلمة المرور للتطبيقات على الخادم - يدعم "وكيل التطبيق" العديد من أوضاع تسجيل الدخول الفردية. إن تسجيل الدخول المستند إلى كلمة المرور مخصص للتطبيقات التي تستخدم تركيبة اسم المستخدم/كلمة المرور للمصادقة. عندما تقوم بتكوين تسجيل الدخول المستند إلى كلمة المرور للتطبيق، يجب على المستخدمين تسجيل الدخول إلى التطبيق داخل التطبيق مرة واحدة. بعد ذلك، يخزن Azure Active Directory معلومات تسجيل الدخول ويوفرها تلقائيا للتطبيق عند وصول المستخدمين إليها عن بعد.
    - يجب أن تكون قد نشرت تطبيقك واختبرته باستخدام وكيل التطبيق. إذا لم يكن الأمر كذلك، فاتبع الخطوات في نشر التطبيقات باستخدام [Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) ثم تابع تكوين SSO المستند إلى كلمة المرور للتطبيقات على الخادم.

استكشاف الأخطاء في تسجيل الدخول الفردي المستند إلى كلمة المرور وإصلاحها، راجع استكشاف الأخطاء وإصلاحها في [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
