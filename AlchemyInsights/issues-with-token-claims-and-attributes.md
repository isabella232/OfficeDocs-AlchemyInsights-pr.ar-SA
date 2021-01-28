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
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="32c63-102">مشاكل تتعلق بمطالبات الرمز المميز وسماته</span><span class="sxs-lookup"><span data-stu-id="32c63-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="32c63-103">**تحديث مطالبات الرمز المميز أو تكوينها أو إزالتها**</span><span class="sxs-lookup"><span data-stu-id="32c63-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="32c63-104">باستخدام Azure Active Directory (Azure AD)، يمكنك تخصيص نوع المطالبة للدور في الرمز المميز للرد الذي تتلقاه بعد تخويل تطبيق. [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)</span><span class="sxs-lookup"><span data-stu-id="32c63-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="32c63-105">يمكن لمطوري التطبيقات استخدام المطالبات الاختيارية في تطبيقات Azure AD الخاصة بهم لتحديد المطالبات التي يريدونها في الرموز المميزة المرسلة إلى التطبيق الخاص بهم.</span><span class="sxs-lookup"><span data-stu-id="32c63-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="32c63-106">لمزيد من المعلومات، راجع ["تقديم مطالبات اختيارية لتطبيقك".](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="32c63-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="32c63-107">[تكوين مطالبات المجموعة للتطبيقات باستخدام Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)</span><span class="sxs-lookup"><span data-stu-id="32c63-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="32c63-108">إذا كنت تستخدم تسجيل الدخول المفرد السلس في التطبيق، فشاهد تخصيص المطالبات الصادرة في الرمز [المميز SAML لتطبيقات المؤسسة.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="32c63-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="32c63-109">**تعيين سمة المطالبات**</span><span class="sxs-lookup"><span data-stu-id="32c63-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="32c63-110">لتكوين نهج تعيين المطالبات باستخدام PowerShell، راجع تخصيص المطالبات التي تصدر في رموز رمزية لتطبيق معين في [مستأجر (معاينة).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)</span><span class="sxs-lookup"><span data-stu-id="32c63-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="32c63-111">توفر سمات ملحق مخطط الدليل طريقة لتخزين بيانات إضافية في Azure Active Directory على كائنات المستخدمين وكائنات الدليل الأخرى مثل المجموعات وتفاصيل المستأجر وأهم الخدمات.</span><span class="sxs-lookup"><span data-stu-id="32c63-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="32c63-112">يمكن استخدام سمات الملحقات فقط على كائنات المستخدمين لادعاءات التطبيقات.</span><span class="sxs-lookup"><span data-stu-id="32c63-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="32c63-113">[يصف استخدام سمات](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) ملحق مخطط الدليل في المطالبات كيفية استخدام سمات ملحق مخطط الدليل لإرسال بيانات المستخدم إلى التطبيقات في مطالبات الرمز المميز.</span><span class="sxs-lookup"><span data-stu-id="32c63-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="32c63-114">لمزيد من المعلومات حول مطالبات الرمز المميز، راجع:</span><span class="sxs-lookup"><span data-stu-id="32c63-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="32c63-115">المطالبات في الرموز المميزة للوصول</span><span class="sxs-lookup"><span data-stu-id="32c63-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="32c63-116">المطالبات في id_token</span><span class="sxs-lookup"><span data-stu-id="32c63-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="32c63-117">[المطالبات](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) التي يمكنك توقعها في رموز الم ID المميزة والوصول المميزة الصادرة عن Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="32c63-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="32c63-118">مرجع مطالبات الرمز المميز SAML</span><span class="sxs-lookup"><span data-stu-id="32c63-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
