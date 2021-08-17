---
title: مشاكل اتصال SSO
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084333"
---
# <a name="sso-connection-issues"></a>مشاكل اتصال SSO

1. اتبع ["Quickstart": تكوين خصائص دليل](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) تطبيق لتكوين التطبيق.
2. استنادا إلى التطبيق و خيار [تسجيل الدخول الفردي](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) الذي اخترته، اتبع الإرشادات المناسبة أدناه:
    - لتكوين تطبيق في الموقع **ل** تسجيل الدخول الفردي المستند إلى **SAML،** راجع [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)تسجيل الدخول المفرد للتطبيقات في الموقع باستخدام وكيل التطبيق .
    - لتكوين تطبيق **سحابة** تسجيل الدخول الفردي المستند إلى كلمة **المرور،** راجع تكوين تسجيل الدخول  [المفرد لكلمة المرور](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - لتكوين تطبيق **في** الموقع للحصول على تسجيل الدخول المفرد من خلال **وكيل** التطبيق، راجع تخزين كلمة المرور ل تسجيل الدخول الفردي [باستخدام وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **استكشاف مشاكل** وكيل التطبيق وإصلاحها : نوصيك ببدء مراجعة تدفق استكشاف [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)الأخطاء وإصلاحها، تصحيح مشاكل موصل وكيل التطبيق ، لتحديد ما إذا تم تكوين موصلات وكيل التطبيق بشكل صحيح. إذا كنت لا تزال تواجه مشكلة في الاتصال بتطبيق، فاتبع تدفق استكشاف الأخطاء وإصلاحها في تصحيح مشاكل تطبيق [وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). يمكنك تحديد [مشاكل CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) باستخدام أدوات تصحيح الأخطاء في المستعرض:
    - قم ب تشغيل المستعرض واستعرض بحثا عن تطبيق الويب.
    - اضغط **على F12** للحصول على وحدة التحكم في تصحيح الأخطاء.
    - حاول إعادة إنتاج المعاملة، وراجع رسالة وحدة التحكم. ينتج عن انتهاك CORS خطأ في وحدة التحكم حول الأصل.
    - لا يمكن حل بعض مشاكل CORS، مثل عندما يعيد تطبيقك login.microsoft.com المصادقة، وتنتهي صلاحية رمز الوصول المميز. فشلت مكالمة CORS بعد ذلك. الحل البديل لهذا السيناريو هو تمديد مدة صلاحية رمز الوصول المميز، لمنع انتهاء صلاحيته أثناء جلسة عمل المستخدم. لمزيد من المعلومات حول كيفية القيام بذلك، راجع عمر الرمز المميز القابل للتكوين [في النظام الأساسي للهويات في Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. استكشاف الأخطاء وإصلاحها تسجيل الدخول الفردي المستند إلى **SAML**: نوصي بالتحقق من مشاكل تسجيل الدخول إلى تطبيقات تسجيل الدخول الفردية المستندة إلى [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)التي تم تكوينها ، للعثور على حلول للمشاكل التي من المرجح أن تواجهها.
5. استكشاف الأخطاء وإصلاحها تسجيل الدخول الفردي المستند إلى كلمة المرور **:** نوصي بالتحقق من استكشاف الأخطاء في تسجيل الدخول الفردي المستند إلى كلمة المرور وإصلاحها في [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)، للعثور على حلول للمشاكل التي من المرجح أن تواجهها.
6. للحصول على مشاكل الاتصال أثناء استخدام VPN، راجع كيفية استخدام تسجيل الدخول الفردي [(SSO) عبر VPN Wi-Fi الاتصال.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
