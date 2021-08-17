---
title: استكشاف مشاكل تسجيل الدخول المفرد السلس (SSO) المستندة إلى OIDC وإصلاحها
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
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105745"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>استكشاف مشاكل تسجيل الدخول المفرد السلس (SSO) المستندة إلى OIDC وإصلاحها

- للتعرف على كيفية إضافة تطبيق مستند إلى OIDC إلى مستأجر Azure، راجع تشغيل سريع: إعداد تسجيل الدخول الفردي (SSO) المستند إلى OIDC لتطبيق في مستأجر [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso).
- للحصول على مزيد من التفاصيل حول التطبيقات التي تستخدم الاتصال OpenID لتطبيق تسجيل الدخول الفردي، راجع فهم تسجيل الدخول الفردي المستند إلى [OIDC](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- للحصول على معلومات في حال اخترت كتابة التعليمات البرمجية عن طريق إرسال طلبات HTTP والتعامل معها مباشرة أو استخدام مكتبة مفتوحة المصدر من جهة خارجية، بدلا من استخدام إحدى مكتباتنا المفتوحة المصدر، راجع [بروتوكولي OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)و OpenID الاتصال على النظام الأساسي للهويات في Microsoft .

**البروتوكولات**

1. [النظام الأساسي للهويات في Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) تدفق المنحة الضمنية والضمنية - إن السمة المميزة للمنحة الضمنية هي أنه يتم إرجاع الرموز المميزة (رموز المرجع المميزة أو رموز الوصول المميزة) مباشرة من نقطة النهاية /تخويل بدلا من نقطة نهاية /token. غالبا ما يتم استخدام هذا كجزء من تدفق رمز التفويض، في ما يسمى **"التدفق المختلط" - استرداد** الرمز المميز للمرجع على طلب /تخويل إلى جانب رمز التفويض . تصف هذه المقالة كيفية إجراء برمجة مباشرة مقابل البروتوكول في التطبيق لطلب الرموز المميزة من Azure AD.
2. النظام الأساسي للهويات في Microsoft التعليمات البرمجية [لتخويل OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - يمكن استخدام منح رمز التخويل OAuth 2.0 في التطبيقات المثبتة على جهاز للوصول إلى الموارد المحمية، مثل واجهات برمجة تطبيقات الويب. باستخدام النظام الأساسي للهويات في Microsoft تطبيق OAuth 2.0، يمكنك إضافة تسجيل الدخول والوصول إلى **API لتطبيقات** الأجهزة المحمولة وسطح المكتب . تصف هذه المقالة كيفية البرمجة مباشرة مقابل البروتوكول في التطبيق باستخدام أي لغة.
3. النظام الأساسي للهويات في Microsoft بروتوكول الاتصال [OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - عند استخدام النظام الأساسي للهويات في Microsoft الخاص بتطبيق OpenID الاتصال، يمكنك إضافة تسجيل الدخول والوصول إلى API لتطبيقاتك. توضح هذه المقالة كيفية القيام بذلك بشكل مستقل عن اللغة وتصف كيفية إرسال رسائل HTTP وتلقيها دون استخدام أي مكتبات **Microsoft مفتوحة المصدر.**
4. النظام الأساسي للهويات في Microsoft وتدفق بيانات اعتماد عميل [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - يمكنك استخدام منح بيانات اعتماد عميل OAuth 2.0 المحدد في RFC 6749، ويسمى أحيانا **OAuth** على قدمين ، للوصول إلى الموارد المستضافة على الويب باستخدام هوية أحد التطبيقات. يستخدم هذا النوع من المنح بشكل شائع لتفاعلات الخادم إلى الخادم التي يجب تشغيلها في الخلفية، دون التفاعل الفوري مع المستخدم. يشار إلى هذه الأنواع من التطبيقات غالبا باسم حسابات الخدمة أو **daemons** **.** تصف هذه المقالة كيفية البرمجة مباشرة مقابل البروتوكول في التطبيق.
