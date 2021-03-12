---
title: استكشاف مشاكل تسجيل الدخول الفردي السلس (SSO) المستندة إلى كلمة المرور وإصلاحها
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
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714664"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="153ee-102">استكشاف مشاكل تسجيل الدخول الفردي السلس (SSO) المستندة إلى كلمة المرور وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="153ee-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="153ee-103">للتعرف على أساسيات SSO المستند إلى كلمة المرور، راجع المصادقة المستندة إلى كلمة المرور [باستخدام Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="153ee-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="153ee-104">**تكوين SSO المستند إلى كلمة المرور**</span><span class="sxs-lookup"><span data-stu-id="153ee-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="153ee-105">[قم بتكوين تسجيل الدخول](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) المفرد المستند إلى كلمة المرور - تدخل هذه المقالة في مزيد من التفاصيل حول خيار تسجيل الدخول الموحد المستند إلى كلمة المرور.</span><span class="sxs-lookup"><span data-stu-id="153ee-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="153ee-106">إذا كان التطبيق الذي تقوم بإضافته يتطلب تكوينا مخصصا وأنت بحاجة إلى استخدام SSO قائم على كلمة المرور، فإن هذه المقالة مخصصة لك.</span><span class="sxs-lookup"><span data-stu-id="153ee-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="153ee-107">[قم بتكوين تسجيل الدخول](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) الفردي المستند إلى كلمة المرور للتطبيقات على الكمبيوتر - يدعم "وكيل التطبيق" العديد من أوضاع تسجيل الدخول المفرد.</span><span class="sxs-lookup"><span data-stu-id="153ee-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="153ee-108">إن تسجيل الدخول المستند إلى كلمة المرور مخصص للتطبيقات التي تستخدم تركيبة اسم المستخدم/كلمة المرور للمصادقة.</span><span class="sxs-lookup"><span data-stu-id="153ee-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="153ee-109">عندما تقوم بتكوين تسجيل الدخول المستند إلى كلمة مرور للتطبيق، يجب على المستخدمين تسجيل الدخول إلى التطبيق في الموقع الإلكتروني مرة واحدة.</span><span class="sxs-lookup"><span data-stu-id="153ee-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="153ee-110">بعد ذلك، يخزن Azure Active Directory معلومات تسجيل الدخول ويوفرها تلقائيا للتطبيق عندما يقوم المستخدمون بالوصول إليها عن بعد.</span><span class="sxs-lookup"><span data-stu-id="153ee-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="153ee-111">كان من المفترض أن تكون قد نشرت تطبيقك واختبرته باستخدام وكيل التطبيق.</span><span class="sxs-lookup"><span data-stu-id="153ee-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="153ee-112">إذا لم يكن الأمر كذلك، فاتبع الخطوات في "نشر التطبيقات" باستخدام وكيل تطبيق [Azure AD،](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) ثم تابع تكوين SSO المستند إلى كلمة المرور للتطبيقات على الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="153ee-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="153ee-113">استكشاف الأخطاء في تسجيل الدخول المفرد المستند إلى كلمة المرور وإصلاحها، راجع استكشاف الأخطاء في تسجيل الدخول الفردي المستند إلى كلمة المرور وإصلاحها [في Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="153ee-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
