---
title: تكوين مدد الرمز المميز وتمديدها
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916653"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="c6ebc-102">تكوين مدد الرمز المميز وتمديدها</span><span class="sxs-lookup"><span data-stu-id="c6ebc-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="c6ebc-103">يمكنك تحديد مده بقاء access أو SAML أو الرمز المميز لمعرف تم إصداره بواسطة النظام الأساسي لهويه Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c6ebc-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="c6ebc-104">يمكنك تعيين اعمار الرموز المميزة لجميع التطبيقات في مؤسستك ، للحصول علي تطبيق متعدد المستاجرين (متعدد المؤسسات) ، أو لحساب خدمه معين في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="c6ebc-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="c6ebc-105">للحصول علي مزيد من المعلومات ، أقرا [اعمار الرموز القابلة للتكوين](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="c6ebc-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="c6ebc-106">للحصول علي أمثله ، أقرا [أمثله حول كيفيه تكوين مدد الرمز المميز](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="c6ebc-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="c6ebc-107">لمعرفه كيفيه تكوين مده بقاء الرمز المميز وتوافقه في Azure Active directory B2C (Azure AD B2C) ، راجع [تكوين الرموز المميزة في Azure active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="c6ebc-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="c6ebc-108">تصف المقالة [تكوين سلوك جلسة العمل في Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) طرق تسجيل الدخول الأحادي (SSO) المستخدمة في AZURE AD B2C وتساعدك علي اختيار أسلوب SSO الأكثر ملاءمة عند تكوين النهج.</span><span class="sxs-lookup"><span data-stu-id="c6ebc-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="c6ebc-109">**ما المدة التي تستغرقها الرموز المميزة في العمل ؟ ما المدة التي يكون فيها صالحا ؟**</span><span class="sxs-lookup"><span data-stu-id="c6ebc-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="c6ebc-110">اعمار الرموز المميزة هي 1 ساعة ومده بقاء جلسة العمل 24 ساعة.</span><span class="sxs-lookup"><span data-stu-id="c6ebc-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="c6ebc-111">وهذا يعني انه إذا لم يتم اجراء اي طلبات في 24 ساعة ، ستحتاج إلى تسجيل الدخول مره أخرى قبل طلب رمز مميز جديد.</span><span class="sxs-lookup"><span data-stu-id="c6ebc-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="c6ebc-112">بعد 30 مايو 2020 ، لن يتمكن اي مستاجر جديد من استخدام نهج عمر الرمز المميز القابل للتكوين لتكوين جلسة العمل وتحديث الرموز المميزة.</span><span class="sxs-lookup"><span data-stu-id="c6ebc-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="c6ebc-113">سيحدث إهمال خلال عده أشهر بعد ذلك ، مما يعني اننا سنقوم بإيقاف جلسة العمل الموجودة هونورينج وتحديث نهج الرموز المميزة.</span><span class="sxs-lookup"><span data-stu-id="c6ebc-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="c6ebc-114">لا يزال بإمكانك تكوين مدد حياه الوصول بعد إهمال.</span><span class="sxs-lookup"><span data-stu-id="c6ebc-114">You can still configure access token lifetimes after the deprecation.</span></span>






