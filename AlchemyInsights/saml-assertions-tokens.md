---
title: تأكيدات SAML (الرموز المميزة)
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
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109227"
---
# <a name="saml-assertions-tokens"></a>تأكيدات SAML (الرموز المميزة)

1. الرموز المميزة لعلامة تأكيدات الأمان (SAML) هي تمثيلات XML للادعاءات. بشكل افتراضي، يتم إصدار Windows المميزة التي تستخدمها مؤسسة الاتصالات (WCF) في سيناريوهات الأمان الخارجية. لمزيد من المعلومات، راجع [رموز SAML المميزة والمطالبات](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. تصدر النظام الأساسي للهويات في Microsoft أنواعا متعددة من رموز الأمان المميزة في معالجة كل تدفق مصادقة. [يصف مرجع مطالبات رموز SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) المميزة تنسيق رموز SAML المميزة ومواصفات أمانها ومحتوياتها.
3. اتبع الإرشادات في عمر الرمز المميز القابل للتكوين [في](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) النظام الأساسي للهويات في Microsoft لفهم كيفية تكوين عمر الرمز المميز.
4. اتبع الخطوات الموضحة في [هذه المقالة](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) لفهم كيفية تكوين تشفير الرمز المميز Azure AD SAML.
5. في Azure AD، يمكنك إعداد خيارات توقيع الشهادة وخوارزمية توقيع الشهادة. لمزيد من المعلومات، راجع خيارات متقدمة لتوقيع الشهادات في [الرمز المميز SAML لتطبيقات المعرض في Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
