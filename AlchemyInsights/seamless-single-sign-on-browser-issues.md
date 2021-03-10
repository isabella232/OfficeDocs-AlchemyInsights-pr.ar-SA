---
title: استكشاف مشاكل مستعرض تسجيل الدخول الفردي السلس (SSO) وإصلاحها
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
- "9377"
ms.openlocfilehash: 507dc5a3bdc5f1bc27cf12865daf98df6c702827
ms.sourcegitcommit: f835aa80f2d85e9c0549be9395110377dba50f3d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692470"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-browser-issues"></a><span data-ttu-id="9428e-102">استكشاف مشاكل مستعرض تسجيل الدخول الفردي السلس (SSO) وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="9428e-102">Troubleshoot Seamless Single Sign-on (SSO) browser issues</span></span>

<span data-ttu-id="9428e-103">يمكن لمعظم المستخدمين حل مشكلة مستعرض SSO السلس باستخدام الخطوات أدناه:</span><span class="sxs-lookup"><span data-stu-id="9428e-103">Most users are able to resolve their Seamless SSO browser issue using the steps below:</span></span>

1. <span data-ttu-id="9428e-104">تأكد من أن المستعرض م حديث.</span><span class="sxs-lookup"><span data-stu-id="9428e-104">Make sure your browser is up-to-date.</span></span>
2. <span data-ttu-id="9428e-105">احذف ملفات تعريف الارتباط من المستعرض لإزالة جلسة تسجيل الدخول الخاصة غير الصالحة وحاول تسجيل الدخول مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="9428e-105">Delete cookies from your browser to remove an invalid SSO session and try logging in again.</span></span>
3. <span data-ttu-id="9428e-106">حاول تسجيل الدخول باستخدام مستعرض آخر.</span><span class="sxs-lookup"><span data-stu-id="9428e-106">Try logging in using a different browser.</span></span>

<span data-ttu-id="9428e-107">**مشاكل المستعرض المعروفة**</span><span class="sxs-lookup"><span data-stu-id="9428e-107">**Known Browser Issues**</span></span>

- <span data-ttu-id="9428e-108">لا يعمل SSO السلس في وضع الاستعراض الخاص في Firefox.</span><span class="sxs-lookup"><span data-stu-id="9428e-108">Seamless SSO doesn't work in private browsing mode on Firefox.</span></span>
- <span data-ttu-id="9428e-109">لا يعمل SSO السلس في Internet Explorer عند تشغيل الوضع المحسن المحمي.</span><span class="sxs-lookup"><span data-stu-id="9428e-109">Seamless SSO doesn't work in Internet Explorer when Enhanced Protected mode is turned on.</span></span>
- <span data-ttu-id="9428e-110">لا يعمل SSO السلس في وضع الاستعراض الخاص على Microsoft Edge (القديم).</span><span class="sxs-lookup"><span data-stu-id="9428e-110">Seamless SSO doesn't work in private browsing mode on Microsoft Edge (legacy).</span></span>
- <span data-ttu-id="9428e-111">لا يعمل SSO السلس على مستعرضات الأجهزة المحمولة على نظامي التشغيل iOS وAndroid.</span><span class="sxs-lookup"><span data-stu-id="9428e-111">Seamless SSO doesn't work on mobile browsers on iOS and Android.</span></span>

<span data-ttu-id="9428e-112">يدعم SSO السلس الإصدار التالي من Microsoft Edge استنادا إلى Chromium ويعمل في وضع InPrivate ووضع الضيف حسب التصميم.</span><span class="sxs-lookup"><span data-stu-id="9428e-112">Seamless SSO supports the next version of Microsoft Edge based on Chromium and it works in InPrivate and Guest mode by design.</span></span>

<span data-ttu-id="9428e-113">**استشارات**</span><span class="sxs-lookup"><span data-stu-id="9428e-113">**Advisory**</span></span>

<span data-ttu-id="9428e-114">للحصول على طلبات ميزات أو طرح أسئلة تقنية حول "SSO السلس"، راجع [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html)</span><span class="sxs-lookup"><span data-stu-id="9428e-114">To make feature requests or ask technical questions about Seamless SSO, see [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html)</span></span>
