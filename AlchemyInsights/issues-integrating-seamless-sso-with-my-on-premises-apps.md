---
title: المشاكل المتعلقة بتكامل SSO السلس مع تطبيقاتي
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028279"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>المشاكل المتعلقة بتكامل SSO السلس مع تطبيقاتي

لا استكشاف المشاكل وإصلاحها مع تكامل SSO السلس مع التطبيقات في الموقع، قم بما يلي:

**الخطوات المستحسنة**

1. لتكوين تطبيق **في** الموقع للحصول على تسجيل الدخول المفرد من خلال **وكيل** التطبيق، راجع تخزين كلمة المرور ل تسجيل الدخول الفردي [باستخدام وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. استكشاف **مشاكل** وكيل التطبيق وإصلاحها : نوصيك ببدء مراجعة تدفق استكشاف [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)الأخطاء وإصلاحها، تصحيح مشاكل موصل وكيل التطبيق ، لتحديد ما إذا تم تكوين موصلات وكيل التطبيق بشكل صحيح. إذا كنت لا تزال تواجه مشكلة في الاتصال بتطبيق، فاتبع خطوات استكشاف الأخطاء وإصلاحها في تصحيح مشاكل تطبيق [وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). يمكنك تحديد [مشاكل CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) باستخدام أدوات تتبع الأخطاء في المستعرض التالية:
    1. قم ب تشغيل المستعرض واستعرض بحثا عن تطبيق الويب.
    1. اضغط **على F12** للحصول على وحدة التحكم في تصحيح الأخطاء.
    1. حاول إعادة إنتاج المعاملة، وراجع رسالة وحدة التحكم. ينتج عن انتهاك CORS خطأ في وحدة التحكم حول الأصل.
    1. لا يمكن حل بعض مشاكل CORS، مثل عند إعادة توجيه تطبيقك إلى login.microsoftonline.com المصادقة، وتنتهي صلاحية رمز الوصول المميز. فشلت مكالمة CORS بعد ذلك. الحل البديل لهذا السيناريو هو تمديد مدة صلاحية رمز الوصول المميز، لمنع انتهاء صلاحيته أثناء جلسة عمل المستخدم. لمزيد من المعلومات حول كيفية القيام بذلك، راجع عمر الرمز المميز القابل للتكوين [في النظام الأساسي للهويات في Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**المستندات المستحسنة**

- [كيفية تكوين تسجيل الدخول الفردي إلى تطبيق وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [تسجيل الدخول المفرد ل SAML للتطبيقات في الموقع باستخدام وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [فهم مشاكل وكيل تطبيق Azure Active Directory CORS وحلها](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [استكشاف الأخطاء في تكوينات الوفود المقيدة لوكيل التطبيق وإصلاحها](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)