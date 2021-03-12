---
title: استكشاف مشاكل تسجيل الدخول الفردي السلس (SSO) المستندة إلى كلمة المرور وإصلاحها
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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714664"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>استكشاف مشاكل تسجيل الدخول الفردي السلس (SSO) المستندة إلى كلمة المرور وإصلاحها

للتعرف على أساسيات SSO المستند إلى كلمة المرور، راجع المصادقة المستندة إلى كلمة المرور [باستخدام Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**تكوين SSO المستند إلى كلمة المرور**

1. [قم بتكوين تسجيل الدخول](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) المفرد المستند إلى كلمة المرور - تدخل هذه المقالة في مزيد من التفاصيل حول خيار تسجيل الدخول الموحد المستند إلى كلمة المرور. إذا كان التطبيق الذي تقوم بإضافته يتطلب تكوينا مخصصا وأنت بحاجة إلى استخدام SSO قائم على كلمة المرور، فإن هذه المقالة مخصصة لك.
2. [قم بتكوين تسجيل الدخول](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) الفردي المستند إلى كلمة المرور للتطبيقات على الكمبيوتر - يدعم "وكيل التطبيق" العديد من أوضاع تسجيل الدخول المفرد. إن تسجيل الدخول المستند إلى كلمة المرور مخصص للتطبيقات التي تستخدم تركيبة اسم المستخدم/كلمة المرور للمصادقة. عندما تقوم بتكوين تسجيل الدخول المستند إلى كلمة مرور للتطبيق، يجب على المستخدمين تسجيل الدخول إلى التطبيق في الموقع الإلكتروني مرة واحدة. بعد ذلك، يخزن Azure Active Directory معلومات تسجيل الدخول ويوفرها تلقائيا للتطبيق عندما يقوم المستخدمون بالوصول إليها عن بعد.
    - كان من المفترض أن تكون قد نشرت تطبيقك واختبرته باستخدام وكيل التطبيق. إذا لم يكن الأمر كذلك، فاتبع الخطوات في "نشر التطبيقات" باستخدام وكيل تطبيق [Azure AD،](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) ثم تابع تكوين SSO المستند إلى كلمة المرور للتطبيقات على الإنترنت.

استكشاف الأخطاء في تسجيل الدخول المفرد المستند إلى كلمة المرور وإصلاحها، راجع استكشاف الأخطاء في تسجيل الدخول الفردي المستند إلى كلمة المرور وإصلاحها [في Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
