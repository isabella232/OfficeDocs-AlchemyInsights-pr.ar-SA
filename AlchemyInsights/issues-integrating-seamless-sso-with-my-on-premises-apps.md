---
title: المشاكل المتعلقة بتكامل SSO السلسة مع التطبيقات المحلية
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868634"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a><span data-ttu-id="48185-102">المشاكل المتعلقة بتكامل SSO السلسة مع التطبيقات المحلية</span><span class="sxs-lookup"><span data-stu-id="48185-102">Issues with integrating Seamless SSO with my on-premises apps</span></span>

<span data-ttu-id="48185-103">لاستكشاف المشاكل المتعلقة بتكامل SSO والتطبيقات المحلية وإصلاحها ، قم بما يلي:</span><span class="sxs-lookup"><span data-stu-id="48185-103">To troubleshoot issues with integrating Seamless SSO with on-premises applications, do the following:</span></span>

<span data-ttu-id="48185-104">**الخطوات الموصي بها**</span><span class="sxs-lookup"><span data-stu-id="48185-104">**Recommended steps**</span></span>

1. <span data-ttu-id="48185-105">لتكوين **تطبيق محلي** **لتسجيل الدخول الأحادي عبر وكيل التطبيق**، راجع [فاولتينج كلمه المرور لتسجيل الدخول الأحادي باستخدام وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span><span class="sxs-lookup"><span data-stu-id="48185-105">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
1. <span data-ttu-id="48185-106">**استكشاف مشاكل وكيل التطبيق وإصلاحها**: من المستحسن ان تبدا بمراجعه تدفق استكشاف الأخطاء وإصلاحها ، [ومشاكل موصل وكيل التطبيق في Debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)، لتحديد ما إذا تم تكوين موصلات وكيل التطبيق بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="48185-106">**Troubleshooting Application Proxy issues**: we recommend that you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="48185-107">إذا كنت لا تزال تواجه مشكله في الاتصال بالتطبيق ، فاتبع خطوات استكشاف الأخطاء وإصلاحها في [تصحيح مشاكل تطبيق وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span><span class="sxs-lookup"><span data-stu-id="48185-107">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="48185-108">يمكنك [تحديد مشاكل كورس](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) باستخدام أدوات تصحيح المستعرض التالية:</span><span class="sxs-lookup"><span data-stu-id="48185-108">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using the following browser debug tools:</span></span>
    1. <span data-ttu-id="48185-109">أبدا تشغيل المستعرض واستعرض وصولا إلى تطبيق ويب.</span><span class="sxs-lookup"><span data-stu-id="48185-109">Launch the browser and browse to the web app.</span></span>
    1. <span data-ttu-id="48185-110">اضغط علي **F12** لإظهار وحده التحكم بالتصحيح.</span><span class="sxs-lookup"><span data-stu-id="48185-110">Press **F12** to bring up the debug console.</span></span>
    1. <span data-ttu-id="48185-111">حاول أعاده إنشاء المعاملة ، ومراجعه رسالة وحده التحكم.</span><span class="sxs-lookup"><span data-stu-id="48185-111">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="48185-112">ينتج انتهاك كورس خطا في وحده التحكم تتعلق بالأصل.</span><span class="sxs-lookup"><span data-stu-id="48185-112">A CORS violation produces a console error about origin.</span></span>
    1. <span data-ttu-id="48185-113">لا يمكن حل بعض مشاكل كورس ، علي سبيل المثال عندما تتم أعاده توجيه التطبيق إلى login.microsoftonline.com للمصادقة عليه ، وتنتهي صلاحيه الرمز المميز للوصول.</span><span class="sxs-lookup"><span data-stu-id="48185-113">Some CORS issues can't be resolved, such as when your app redirects to login.microsoftonline.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="48185-114">ستفشل مكالمة كورس.</span><span class="sxs-lookup"><span data-stu-id="48185-114">The CORS call then fails.</span></span> <span data-ttu-id="48185-115">الحل البديل لهذا السيناريو هو تمديد مده بقاء الرمز المميز للوصول ، لمنع انتهاء صلاحيته اثناء جلسة المستخدم.</span><span class="sxs-lookup"><span data-stu-id="48185-115">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="48185-116">للحصول علي مزيد من المعلومات حول كيفيه القيام بذلك ، راجع فترات [بقاء الرموز القابلة للتكوين في النظام الأساسي للهوية في Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="48185-116">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="48185-117">**المستندات المستحسنة**</span><span class="sxs-lookup"><span data-stu-id="48185-117">**Recommended documents**</span></span>

- [<span data-ttu-id="48185-118">كيفيه تكوين تسجيل الدخول الأحادي إلى تطبيق وكيل التطبيق</span><span class="sxs-lookup"><span data-stu-id="48185-118">How to configure single sign-on to an Application Proxy application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [<span data-ttu-id="48185-119">SAML تسجيل الدخول الأحادي للتطبيقات المحلية باستخدام وكيل التطبيق</span><span class="sxs-lookup"><span data-stu-id="48185-119">SAML single sign-on for on-premises applications with Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [<span data-ttu-id="48185-120">فهم مشاكل كورس وكيل تطبيق Active Directory وحلها</span><span class="sxs-lookup"><span data-stu-id="48185-120">Understand and solve Azure Active Directory Application Proxy CORS issues</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [<span data-ttu-id="48185-121">استكشاف أخطاء تكوينات التفويض المقيدة ل Kerberos لوكيل التطبيق وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="48185-121">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)