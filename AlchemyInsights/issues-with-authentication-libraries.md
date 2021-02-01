---
title: مشاكل تتعلق بمكتبات المصادقة
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063574"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="f1cd7-102">مشاكل تتعلق بمكتبات المصادقة</span><span class="sxs-lookup"><span data-stu-id="f1cd7-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="f1cd7-103">[تسرد مكتبات مصادقة](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) النظام الأساسي لهوية Microsoft مكتبات برامج وسطى ومدعمة من Microsoft ومتوافقة.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="f1cd7-104">تدعم مكتبة مصادقة Microsoft (MSAL) العديد من تدفقات المصادقة [لاستخدامها](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) في سيناريوهات تطبيق مختلفة.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="f1cd7-105">لمصادقة الرموز المميزة والحصول عليها، يمكنك تهيي تطبيق عميل عام أو سري جديد في التعليمات البرمجية.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="f1cd7-106">يمكنك تعيين عدة خيارات تكوين عند تهيئة تطبيق العميل في مكتبة مصادقة Microsoft (MSAL).</span><span class="sxs-lookup"><span data-stu-id="f1cd7-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="f1cd7-107">لمعرفة المزيد، راجع [خيارات تكوين التطبيق.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)</span><span class="sxs-lookup"><span data-stu-id="f1cd7-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="f1cd7-108">**نهاية دعم Azure Active Directory Authentication Library (ADAL) و Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="f1cd7-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="f1cd7-109">**بدءا من 30 يونيو 2020،** لن نضيف أي ميزات جديدة إلى ADAL و Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="f1cd7-110">سنستمر في تقديم الدعم الفني وتحديثات الأمان ولكننا لن نقدم تحديثات للميزات بعد الآن.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="f1cd7-111">**اعتبارا من 30 يونيو 2022،** سننهي دعم ADAL و Azure AD Graph ولن نوفر تحديثات الدعم التقني أو الأمان.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="f1cd7-112">ستستمر التطبيقات التي تستخدم ADAL على إصدارات نظام التشغيل الموجودة في العمل بعد هذا الوقت ولكنها لن تحصل على أي تحديثات للدعم التقني *أو الأمان.*</span><span class="sxs-lookup"><span data-stu-id="f1cd7-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="f1cd7-113">قد لا تتلقى التطبيقات التي تستخدم Azure AD Graph بعد هذا الوقت استجابات من نقطة نهاية Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="f1cd7-114">**ترحيل ADAL**</span><span class="sxs-lookup"><span data-stu-id="f1cd7-114">**ADAL Migration**</span></span>

<span data-ttu-id="f1cd7-115">نوصي بالتحديث إلى [مكتبة مصادقة Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)، التي تحتوي على أحدث الميزات وتحديثات الأمان.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="f1cd7-116">إذا كنت تستخدم تطبيقات Microsoft، فتعرف على أن Microsoft تقوم بتقليل تطبيقاتها إلى MSAL بحلول الموعد النهائي لنهاية الدعم، مع التأكد من أنها ستستفيد من تحسينات الميزات والأمان المستمرة في MSAL.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="f1cd7-117">لمزيد من المعلومات، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="f1cd7-117">For more information, see:</span></span>

1. [<span data-ttu-id="f1cd7-118">قراءة الأسئلة الشائعة حول ADAL</span><span class="sxs-lookup"><span data-stu-id="f1cd7-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="f1cd7-119">تعرّف على كيفية ترحيل التطبيقات على أساس كل نظام أساسي</span><span class="sxs-lookup"><span data-stu-id="f1cd7-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="f1cd7-120">إذا احتجت إلى مساعدة في فهم التطبيقات التي تستخدم ADAL، فإننا ننصحك بمراجعة كل التعليمات البرمجية المصدر للتطبيقات، وإذا كان ذلك قابلا للتطبيق، فصل إلى أي موفري خدمات الإنترنت أو موفري التطبيقات.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="f1cd7-121">يمكن أن يوفر لك دعم Microsoft أيضًا قائمة بجميع تطبيقات ADAL غير التابعة لـ Microsoft في المستأجر الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="f1cd7-122">**ترحيل AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="f1cd7-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="f1cd7-123">بالنسبة للتطبيقات التي تستخدم Azure AD Graph، اتبع الإرشادات الخاصة بترحيل تطبيقات [Azure AD Graph إلى Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="f1cd7-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="f1cd7-124">توفر قائمة اختيار الترحيل نقطة بدء.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="f1cd7-125">يُُظهر مدخل تسجيل تطبيق Azure التطبيقات التي تستخدم AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="f1cd7-126">نوصيك بمراجعة جميع التعليمات البرمجية المصدر لتطبيقاتك، وإذا أمكن، يمكنك الوصول إلى أي من موردي البرامج المستقلين أو مزودي التطبيقات.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="f1cd7-127">يمكن أن يوفر لك دعم Microsoft أيضا قائمة بجميع استخدام AAD Graph في المستأجر الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="f1cd7-128">لكي يمكن لتطبيقك الوصول إلى البيانات في Microsoft Graph، يجب على المستخدم أو المسؤول منحه الأذونات الصحيحة عبر عملية موافقة.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="f1cd7-129">يسرد [مرجع أذونات Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) الأذونات المقترنة بكل مجموعة رئيسية من واجهات برمجة تطبيقات Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="f1cd7-130">كما يوفر إرشادات حول كيفية استخدام الأذونات.</span><span class="sxs-lookup"><span data-stu-id="f1cd7-130">It also provides guidance about how to use the permissions.</span></span>
