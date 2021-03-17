---
title: تكوين تسجيل الدخول الفردي السلس (SSO)
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
- "9004344"
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841386"
---
# <a name="configure-seamless-single-sign-on-sso"></a>تكوين تسجيل الدخول الفردي السلس (SSO)

**تكوين التطبيقات**

1. يجب أن تحصل على القيم من مورد التطبيق. يمكنك إدخال القيم يدويا أو تحميل ملف بيانات تعريف لاستخراج قيمة الحقول.
2. تم بالفعل تكوين العديد من التطبيقات مسبقا للعمل مع Azure AD. يتم سرد هذه التطبيقات في معرض التطبيقات التي يمكنك استعراضها عند إضافة تطبيق إلى مستأجر Azure AD. [تقربك سلسلة](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) "العمل السريع" خلال العملية.
3. لإنشاء تطبيق غير معرض، يمكنك النقر فوق + الزر إنشاء **تطبيق** خاص بك وإعطاء اسم للتطبيق.
    - بشكل افتراضي، سيتم تحديد **دمج** أي تطبيق آخر لم تعثر عليه في المعرض وهو الخيار الصحيح للتطبيقات غير المعرضية.
    - بمجرد الضغط على **إنشاء** بعد وضع اسم التطبيق، سيتم إنشاء تطبيق مؤسسة جديد غير معرض.
    - بعد ذلك، يمكنك الانتقال إلى  **تسجيل الدخول** المفرد ضمن إدارة هذا التطبيق وستتمكن من رؤية أساليب مختلفة لتنفيذه في بيئتك.

**تكوين SSO السلس لتطبيق معين**

بالنسبة للتطبيقات في المعرض، ستجد إرشادات مفصلة خطوة بخطوة. للوصول إلى الخطوات، يمكنك استعراض قائمة بكل برامج تكوين التطبيق التعليمية في [برامج SaaS التعليمية لتكوين تطبيق](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**تكوين SSO المستند إلى SAML**

1. Quickstart: إعداد تسجيل الدخول الفردي (SSO) المستند إلى SAML لتطبيق في [مستأجر Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso).
2. لمعرفة المزيد حول الخيار المستند إلى SAML ل تسجيل الدخول الفردي، راجع فهم تسجيل الدخول الفردي المستند إلى [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. للتعرف على طلبات مصادقة SAML 2.0 والاستجابات التي يدعمها Azure Active Directory (Azure AD) ل Single Sign-On (SSO)، راجع بروتوكول SINGLE [Sign-On SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. للتعرف على كيفية إنشاء تسجيل الدخول الفردي (SSO) المستند إلى SAML وتكوينه لتطبيقك في Azure Active Directory (Azure AD) باستخدام Microsoft Graph API، راجع تكوين تسجيل الدخول الفردي المستند إلى SAML لتطبيقك باستخدام API ل [Microsoft Graph](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. لمعرفة كيفية استخدام Azure AD لبروتوكول SAML، راجع كيفية استخدام النظام الأساسي [لهوية Microsoft لبروتوكول SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**تكوين الرموز المميزة والمطالبات**

1. [كيفية: تخصيص المطالبات الصادرة في الرمز المميز SAML للتطبيقات الخاصة بالمؤسسات](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. للتعرف على كيفية تكوين المطالبات باستخدام PowerShell، راجع كيفية: تخصيص المطالبات المنبعثة في الرموز المميزة لتطبيق معين في [مستأجر (معاينة)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. للتعرف على كيفية تكوين المطالبات الاختيارية، راجع [كيفية: تقديم مطالبات اختيارية لتطبيقك](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. للتعرف على كيفية استخدام سمات ملحق مخطط الدليل لإرسال بيانات المستخدم إلى التطبيقات في مطالبات الرمز المميز، راجع استخدام سمات ملحق مخطط [الدليل في المطالبات](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. للتعرف على كيفية تكوين عمر الرمز المميز، راجع عمر الرمز المميز القابل للتكوين في النظام الأساسي [لهوية Microsoft (معاينة)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. تكوين نهج مدة حياة الرمز [المميز (معاينة)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - في هذه المقالة، نستعرض سيناريو نهج شائع يمكن أن يساعدك على فرض قواعد جديدة لمدى عمر الرمز المميز. في المثال، ستتعرف على كيفية إنشاء نهج يتطلب من المستخدمين المصادقة بشكل متكرر أكثر في تطبيق الويب.

**استكشاف الأخطاء في تكوين SSO وإصلاحها**

- للحصول على الأسئلة التي يتم طرحها بشكل متكرر حول Azure Active Directory تسجيل الدخول الفردي السلس Sign-On (تسجيل الدخول الموحد السلس)، راجع [Azure Active Directory تسجيل](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)الدخول الفردي السلس: الأسئلة التي يتم طرحها بشكل متكرر .
- للحصول على معلومات حول استكشاف الأخطاء وإصلاحها حول المشاكل الشائعة المتعلقة ب Azure Active Directory (Azure AD) تسجيل الدخول الفردي السلس Sign-On (تسجيل الدخول السلس)، راجع استكشاف الأخطاء [وإصلاحها في Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)تسجيل الدخول الفردي السلس .
