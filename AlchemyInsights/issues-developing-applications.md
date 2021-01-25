---
title: المشاكل المتعلقة بتطوير التطبيقات
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974158"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="7d4ea-102">المشاكل المتعلقة بتطوير التطبيقات</span><span class="sxs-lookup"><span data-stu-id="7d4ea-102">Issues developing applications</span></span>

<span data-ttu-id="7d4ea-103">لاستكشاف المشاكل الأكثر شيوعا عند إنشاء تطبيقات Azure Active directory (AD) ، راجع المقالات التالية:</span><span class="sxs-lookup"><span data-stu-id="7d4ea-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="7d4ea-104">اري صعوبة في تسجيل الدخول إلى التطبيق (التطبيقات) باستخدام مستعرض Chrome فقط</span><span class="sxs-lookup"><span data-stu-id="7d4ea-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="7d4ea-105">لا اعرف كيفيه تغيير الإعدادات الافتراضية لمده بقاء الرمز المميز للتطبيق</span><span class="sxs-lookup"><span data-stu-id="7d4ea-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="7d4ea-106">لا تخلط عن كيفيه عمل الموافقة علي التطبيق</span><span class="sxs-lookup"><span data-stu-id="7d4ea-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="7d4ea-107">لا اعرف كيفيه منح الأذونات إلى التطبيق الخاص بي</span><span class="sxs-lookup"><span data-stu-id="7d4ea-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="7d4ea-108">لا أدرك الفرق بين أذونات التطبيق والمفوض</span><span class="sxs-lookup"><span data-stu-id="7d4ea-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="7d4ea-109">\***نهاية دعم مكتبه المصادقة ل Azure active directory (ADAL) و AZURE AD GRAPH API (رسم بياني AAD)** _</span><span class="sxs-lookup"><span data-stu-id="7d4ea-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="7d4ea-110">بدءا من 30 يونيو 2020 ، فلن نضيف اي ميزات جديده إلى مكتبه مصادقه Azure Active directory (ADAL) و Azure AD Graph API (رسم بياني ل AAD).</span><span class="sxs-lookup"><span data-stu-id="7d4ea-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="7d4ea-111">سنستمر في توفير الدعم التقني وتحديثات الأمان ولكنه لن يوفر تحديثات الميزات بعد الآن.</span><span class="sxs-lookup"><span data-stu-id="7d4ea-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="7d4ea-112">بدءا من 30 يونيو 2022 ، سنقوم بإنهاء الدعم ل ADAL و AAD الرسم البياني ولن يوفر الدعم التقني أو تحديثات الأمان.</span><span class="sxs-lookup"><span data-stu-id="7d4ea-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="7d4ea-113">نتيجة لهذا الشرط ، ما يلي:</span><span class="sxs-lookup"><span data-stu-id="7d4ea-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="7d4ea-114">ستستمر التطبيقات التي تستخدم ADAL في إصدارات نظام التشغيل الموجودة في العمل بعد هذه المرة ولكن لن تحصل علي اي دعم تقني أو تحديثات أمان.</span><span class="sxs-lookup"><span data-stu-id="7d4ea-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="7d4ea-115">قد لا تتلقي التطبيقات التي تستخدم الرسم البياني AAD بعد هذه الفترة الاستجابات من نقطه نهاية الرسم البياني في AAD</span><span class="sxs-lookup"><span data-stu-id="7d4ea-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="7d4ea-116">_ *الترحيل ADAL*\*</span><span class="sxs-lookup"><span data-stu-id="7d4ea-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="7d4ea-117">إذا كنت تستخدم تطبيقات Microsoft ، فنوصي بالتحديث إلى مكتبه مصادقه Microsoft (مسال) ، التي تتضمن أحدث الميزات وتحديثات الأمان.</span><span class="sxs-lookup"><span data-stu-id="7d4ea-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="7d4ea-118">هذه التوصية في سياق Microsoft لبدء عمليه ترحيل تطبيقاته إلى مسال بواسطة الموعد النهائي لنهاية الدعم.</span><span class="sxs-lookup"><span data-stu-id="7d4ea-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="7d4ea-119">تضمن الترحيل بواسطة Microsoft من تطبيقاته مسال التطبيقات مزايا الأمان وتحسينات الميزات التي مسالها.</span><span class="sxs-lookup"><span data-stu-id="7d4ea-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="7d4ea-120">قراءه الاسئله المتداولة حول ADAL</span><span class="sxs-lookup"><span data-stu-id="7d4ea-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="7d4ea-121">تعرف علي كيفيه ترحيل التطبيقات علي أساس لكل نظام أساسي</span><span class="sxs-lookup"><span data-stu-id="7d4ea-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="7d4ea-122">إذا كنت بحاجه إلى مساعده في فهم اي من تطبيقاتك تستخدم ADAL ، فنحن ننصحك بمراجعه كل التعليمات البرمجية المصدر لتطبيقاتك ، ويمكنك الوصول إلى اي من بائعي البرامج المستقلين (إيسفس) أو موفري التطبيقات.</span><span class="sxs-lookup"><span data-stu-id="7d4ea-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="7d4ea-123">يمكن ان يوفر لك دعم Microsoft أيضا قائمه بكل تطبيقات ADAL التابعة ل Microsoft في نطاق المستاجر الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="7d4ea-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="7d4ea-124">**ترحيل الرسم البياني AAD**</span><span class="sxs-lookup"><span data-stu-id="7d4ea-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="7d4ea-125">بالنسبة إلى التطبيقات التي تستخدم الرسم البياني AAD ، اتبع الإرشادات الخاصة بنا لترحيل تطبيقات الرسم البياني AAD إلى Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="7d4ea-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="7d4ea-126">[توفر قائمه الاختيار الخاصة بالترحيل نقطه بدء](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="7d4ea-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="7d4ea-127">يعرض مدخل تسجيلك في Azure app التطبيقات التي تستخدم الرسم البياني AAD.</span><span class="sxs-lookup"><span data-stu-id="7d4ea-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="7d4ea-128">نوصي بمراجعه كل التعليمات البرمجية المصدر لتطبيقاتك ، ويمكنك الوصول إلى اي بائعين مستقلين (إيسفس) أو موفري التطبيقات ، إذا كان ذلك ممكنا.</span><span class="sxs-lookup"><span data-stu-id="7d4ea-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="7d4ea-129">يمكن ان يوفر لك دعم Microsoft أيضا معلومات حول استخدام الرسم البياني AAD في نطاق المستاجر الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="7d4ea-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







