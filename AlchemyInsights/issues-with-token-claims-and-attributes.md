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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035818"
---
# <a name="issues-with-token-claims-and-attributes"></a>مشاكل تتعلق بمطالبات الرمز المميز وسماته

**تحديث مطالبات الرمز المميز أو تكوينها أو إزالتها**

1. باستخدام Azure Active Directory (Azure AD)، يمكنك تخصيص نوع المطالبة للدور في الرمز المميز للرد الذي تتلقاه بعد تخويل تطبيق. [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)
2. يمكن لمطوري التطبيقات استخدام المطالبات الاختيارية في تطبيقات Azure AD الخاصة بهم لتحديد المطالبات التي يريدونها في الرموز المميزة المرسلة إلى التطبيق الخاص بهم. لمزيد من المعلومات، راجع ["تقديم مطالبات اختيارية لتطبيقك".](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [تكوين مطالبات المجموعة للتطبيقات باستخدام Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. إذا كنت تستخدم تسجيل الدخول المفرد السلس في التطبيق، فشاهد تخصيص المطالبات الصادرة في الرمز [المميز SAML لتطبيقات المؤسسة.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**تعيين سمة المطالبات**

1. لتكوين نهج تعيين المطالبات باستخدام PowerShell، راجع تخصيص المطالبات التي تصدر في رموز رمزية لتطبيق معين في [مستأجر (معاينة).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. توفر سمات ملحق مخطط الدليل طريقة لتخزين بيانات إضافية في Azure Active Directory على كائنات المستخدمين وكائنات الدليل الأخرى مثل المجموعات وتفاصيل المستأجر وأهم الخدمات. يمكن استخدام سمات الملحقات فقط على كائنات المستخدمين لادعاءات التطبيقات. [يصف استخدام سمات](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) ملحق مخطط الدليل في المطالبات كيفية استخدام سمات ملحق مخطط الدليل لإرسال بيانات المستخدم إلى التطبيقات في مطالبات الرمز المميز.

لمزيد من المعلومات حول مطالبات الرمز المميز، راجع:

- [المطالبات في الرموز المميزة للوصول](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [المطالبات في id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [المطالبات](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) التي يمكنك توقعها في رموز الم ID المميزة والوصول المميزة الصادرة عن Azure AD B2C
- [مرجع مطالبات الرمز المميز SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
