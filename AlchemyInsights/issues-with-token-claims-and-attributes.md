---
title: مشاكل تتعلق بمطالبات الرمز المميز وسماته
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012871"
---
# <a name="issues-with-token-claims-and-attributes"></a>مشاكل تتعلق بمطالبات الرمز المميز وسماته

**تحديث مطالبات الرموز المميزة أو تكوينها أو إزالتها**

1. باستخدام Azure Active Directory (Azure AD)، يمكنك تخصيص نوع المطالبة لمطالبة الدور في رمز الاستجابة المميز الذي تتلقاه بعد تخويل تطبيق. [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)
2. يمكن لمطوري التطبيقات استخدام المطالبات الاختيارية في تطبيقات Azure AD لتحديد المطالبات التي يريدونها في الرموز المميزة المرسلة إلى تطبيقهم. لمزيد من المعلومات، راجع [تقديم مطالبات اختيارية لتطبيقك](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [تكوين مطالبات المجموعة للتطبيقات باستخدام Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. إذا كنت تستخدم تسجيل الدخول المفرد السلس في التطبيق، فشاهد تخصيص المطالبات الصادرة [في الرمز المميز SAML لتطبيقات المؤسسة](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**تعيين سمة المطالبات**

1. لتكوين نهج تعيين المطالبات باستخدام PowerShell، راجع تخصيص المطالبات المنبعثة من الرموز المميزة لتطبيق معين في [مستأجر (معاينة)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. توفر سمات ملحقات مخطط الدليل طريقة لتخزين بيانات إضافية في Azure Active Directory على كائنات المستخدمين وكائنات الدليل الأخرى مثل المجموعات وتفاصيل المستأجر وأشياء الخدمة الأساسية. يمكن استخدام سمات الملحقات فقط على كائنات المستخدمين لبعث دعاوى للتطبيقات. [يصف استخدام سمات ملحقات](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) مخطط الدليل في المطالبات كيفية استخدام سمات ملحق مخطط الدليل لإرسال بيانات المستخدم إلى التطبيقات في مطالبات الرموز المميزة.

لمزيد من المعلومات حول مطالبات الرمز المميز، راجع:

- [المطالبات في رموز الوصول المميزة](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [المطالبات في id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [الادعاءات](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) التي يمكنك توقعها في الرموز المميزة ل ID والوصول إلى الرموز المميزة الصادرة عن Azure AD B2C
- [مرجع مطالبات الرمز المميز ل SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
