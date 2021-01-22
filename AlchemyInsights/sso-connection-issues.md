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
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935070"
---
# <a name="sso-connection-issues"></a>مشاكل اتصال SSO

1. اتبع ["Quickstart": تكوين خصائص دليل التطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) لتكوين التطبيق.
2. استنادا إلى التطبيق وخيار تسجيل [الدخول الفردي](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) الذي اخترته، اتبع الإرشادات المناسبة أدناه:
    - لتكوين تطبيق  موقع لتطبيق تسجيل الدخول الفردي المستند إلى **SAML،** راجع تسجيل الدخول المفرد ل SAML للتطبيقات في الموقع مع [وكيل التطبيق.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - لتكوين تطبيق **سحابي** من **أجل** تسجيل الدخول الفردي المستند إلى كلمة المرور، راجع "تكوين تسجيل الدخول الفردي [لكلمة المرور".](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - لتكوين تطبيق **مكاني للحصول** على تسجيل الدخول الفردي من خلال وكيل التطبيق، راجع تخزين كلمة المرور تسجيل الدخول المفرد [باستخدام وكيل التطبيق.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **استكشاف مشاكل** وكيل التطبيق وإصلاحها: نوصيك ببدء مراجعة تدفق استكشاف [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)الأخطاء وإصلاحها، وإصلاح مشاكل موصل وكيل التطبيق، لتحديد ما إذا تم تكوين موصلات وكيل التطبيق بشكل صحيح. إذا كنت لا تزال تواجه مشكلة في الاتصال بتطبيق، فاتبع تدفق استكشاف الأخطاء وإصلاحها في مشاكل تطبيق وكيل [تطبيق Debug.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) يمكنك تحديد [مشاكل CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) باستخدام أدوات تصحيح الأخطاء في المستعرض:
    - قم ب تشغيل المستعرض واستعرض بحثا عن تطبيق الويب.
    - اضغط **على F12** للحصول على وحدة التحكم في تصحيح الأخطاء.
    - حاول إعادة إنتاج المعاملة، وراجع رسالة وحدة التحكم. ينتج عن مخالفة CORS خطأ في وحدة التحكم حول الأصل.
    - لا يمكن حل بعض مشاكل CORS، مثل عندما يعيد تطبيقك التوجيه إلى login.microsoft.com المصادقة، وتنتهي صلاحية الرمز المميز للوصول. فشلت مكالمة CORS بعد ذلك. يوجد حل بديل لهذا السيناريو وهو تمديد مدة صلاحية الرمز المميز للوصول لمنع انتهاء صلاحيته أثناء جلسة عمل المستخدم. لمزيد من المعلومات حول كيفية القيام بذلك، راجع مدة عمر الرمز المميز القابل للتكوين [في النظام الأساسي لهوية Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. استكشاف الأخطاء وإصلاحها باستخدام تسجيل الدخول الفردي المستند إلى **SAML**: نوصي بالتحقق من مشاكل تسجيل الدخول إلى تطبيقات تسجيل الدخول الفردية المستندة إلى [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)التي تم تكوينها، للعثور على حلول للمشاكل التي من المرجح أن تواجهها.
5. **استكشاف** الأخطاء وإصلاحها باستخدام تسجيل الدخول الفردي المستند إلى كلمة المرور: نوصي بالتحقق من تسجيل الدخول الفردي المستند إلى كلمة المرور وإصلاحها في [Azure AD،](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)للعثور على حلول للمشاكل التي من المرجح أن تواجهها.
6. للحصول على مشاكل الاتصال أثناء استخدام VPN، راجع كيفية استخدام تسجيل الدخول الفردي [(SSO)](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)عبر VPN Wi-Fi الاتصال.
