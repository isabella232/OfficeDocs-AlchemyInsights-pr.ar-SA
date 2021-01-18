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
# <a name="saml-assertions-tokens"></a><span data-ttu-id="2a53d-102">تاكيدات SAML (رموز مميزه)</span><span class="sxs-lookup"><span data-stu-id="2a53d-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="2a53d-103">تاكيدات الأمان الرموز المميزة للغة التمييز (SAML) هي تمثيلات XML للمطالبات.</span><span class="sxs-lookup"><span data-stu-id="2a53d-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="2a53d-104">بشكل افتراضي ، يتم إصدار الرموز المميزة لSAML التي تستخدم Windows Communication Foundation (WCF) في سيناريوهات الأمان المتحدة.</span><span class="sxs-lookup"><span data-stu-id="2a53d-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="2a53d-105">لمزيد من المعلومات ، راجع [الرموز المميزة والمطالبات في SAML](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span><span class="sxs-lookup"><span data-stu-id="2a53d-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="2a53d-106">يقوم النظام الأساسي لهويه Microsoft بملء أنواع متعددة من رموز الأمان في معالجه كل تدفق مصادقه.</span><span class="sxs-lookup"><span data-stu-id="2a53d-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="2a53d-107">[SAML يشير إلى مرجع الرموز المميزة](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) لSAML والتنسيق وسمات الأمان ومحتويات الرموز المميزة في 2.0.</span><span class="sxs-lookup"><span data-stu-id="2a53d-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="2a53d-108">اتبع الإرشادات الموجودة في [مده بقاء الرمز المميز القابل للتكوين في النظام الأساسي لهويه Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) للتعرف علي كيفيه تكوين مدد الرمز المميز.</span><span class="sxs-lookup"><span data-stu-id="2a53d-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="2a53d-109">اتبع الخطوات [المذكورة في هذه المقالة](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) لفهم كيفيه تكوين تشفير الرمز المميز AZURE AD SAML.</span><span class="sxs-lookup"><span data-stu-id="2a53d-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="2a53d-110">في Azure AD ، يمكنك اعداد خيارات توقيع الشهادات وخوارزميه توقيع الشهادة.</span><span class="sxs-lookup"><span data-stu-id="2a53d-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="2a53d-111">لمزيد من المعلومات ، راجع [الخيارات المتقدمة لتوقيع الشهادات في الرمز المميز لSAML لتطبيقات المعرض في Azure Active](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)directory.</span><span class="sxs-lookup"><span data-stu-id="2a53d-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
