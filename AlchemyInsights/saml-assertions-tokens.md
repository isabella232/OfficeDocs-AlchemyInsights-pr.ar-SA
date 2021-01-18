---
title: تاكيدات SAML (رموز مميزه)
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
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884805"
---
# <a name="saml-assertions-tokens"></a>تاكيدات SAML (رموز مميزه)

1. تاكيدات الأمان الرموز المميزة للغة التمييز (SAML) هي تمثيلات XML للمطالبات. بشكل افتراضي ، يتم إصدار الرموز المميزة لSAML التي تستخدم Windows Communication Foundation (WCF) في سيناريوهات الأمان المتحدة. لمزيد من المعلومات ، راجع [الرموز المميزة والمطالبات في SAML](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. يقوم النظام الأساسي لهويه Microsoft بملء أنواع متعددة من رموز الأمان في معالجه كل تدفق مصادقه. [SAML يشير إلى مرجع الرموز المميزة](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) لSAML والتنسيق وسمات الأمان ومحتويات الرموز المميزة في 2.0.
3. اتبع الإرشادات الموجودة في [مده بقاء الرمز المميز القابل للتكوين في النظام الأساسي لهويه Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) للتعرف علي كيفيه تكوين مدد الرمز المميز.
4. اتبع الخطوات [المذكورة في هذه المقالة](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) لفهم كيفيه تكوين تشفير الرمز المميز AZURE AD SAML.
5. في Azure AD ، يمكنك اعداد خيارات توقيع الشهادات وخوارزميه توقيع الشهادة. لمزيد من المعلومات ، راجع [الخيارات المتقدمة لتوقيع الشهادات في الرمز المميز لSAML لتطبيقات المعرض في Azure Active](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)directory.
