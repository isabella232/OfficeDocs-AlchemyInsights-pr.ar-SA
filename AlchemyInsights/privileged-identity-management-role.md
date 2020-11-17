---
title: دور أداره الهويات المميزة
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088484"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="ad787-102">دور أداره الهويات المميزة (بيم)</span><span class="sxs-lookup"><span data-stu-id="ad787-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="ad787-103">**لا يتم منح الأذونات بعد تنشيط دور**</span><span class="sxs-lookup"><span data-stu-id="ad787-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="ad787-104">عند تنشيط دور في أداره الهويات المميزة في Azure AD (بيم) ، قد لا يتم نشر التنشيط فورا إلى كل المداخل التي تتطلب الدور المميز.</span><span class="sxs-lookup"><span data-stu-id="ad787-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="ad787-105">في بعض الأحيان ، حتى إذا تم نشر التغيير ، فقد يؤدي التخزين المؤقت لويب في المدخل إلى عدم تاثير التغييرات علي الفور.</span><span class="sxs-lookup"><span data-stu-id="ad787-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="ad787-106">إذا تم تاجيل التنشيط ، فاتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="ad787-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="ad787-107">تسجيل الخروج من مدخل Azure ثم تسجيل الدخول مجددا.</span><span class="sxs-lookup"><span data-stu-id="ad787-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="ad787-108">عند تنشيط دور Azure AD أو دور موارد Azure ، ستري مراحل عمليه التنشيط.</span><span class="sxs-lookup"><span data-stu-id="ad787-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="ad787-109">بمجرد اكتمال كل المراحل ، ستري الارتباط "تسجيل الخروج".</span><span class="sxs-lookup"><span data-stu-id="ad787-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="ad787-110">يمكنك استخدام هذا الارتباط لتسجيل الخروج. سيؤدي ذلك إلى حل معظم حالات تاخير التنشيط.</span><span class="sxs-lookup"><span data-stu-id="ad787-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="ad787-111">في بيم ، تاكد من انك قد أدرجت كعضو في الدور.</span><span class="sxs-lookup"><span data-stu-id="ad787-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="ad787-112">إذا كنت تقوم بتنشيط دور مسؤول Exchange ، فتاكد من تسجيل الخروج وتسجيل الدخول مره أخرى.</span><span class="sxs-lookup"><span data-stu-id="ad787-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="ad787-113">إذا استمرت المشكلة ، فقم بفتح بطاقة دعم ورفع المشكلة.</span><span class="sxs-lookup"><span data-stu-id="ad787-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="ad787-114">إذا كنت تستخدم دور مسؤول Exchange للوصول إلى مركز الأمان والتوافق ، فراجع الخطوة التالية.</span><span class="sxs-lookup"><span data-stu-id="ad787-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="ad787-115">إذا كنت تقوم بتنشيط دور للوصول إلى مركز الأمان والتوافق أو إذا كنت تقوم بتنشيط دور مسؤول SharePoint ، ستواجه بعض التاخير في التنشيط خلال دقائق قليله تصل إلى بضع ساعات.</span><span class="sxs-lookup"><span data-stu-id="ad787-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="ad787-116">هذه مشكله معروفه ونحن نعمل باستمرار مع هذه الفرق لحل هذه المشكلة بأسرع وقت ممكن.</span><span class="sxs-lookup"><span data-stu-id="ad787-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="ad787-117">لمزيد من المعلومات، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="ad787-117">For more information, see:</span></span>

- [<span data-ttu-id="ad787-118">تنشيط ادوار Azure AD الخاصة بي في بيم</span><span class="sxs-lookup"><span data-stu-id="ad787-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="ad787-119">تنشيط ادوار موارد Azure في بيم</span><span class="sxs-lookup"><span data-stu-id="ad787-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="ad787-120">**لا تتم أزاله الأذونات بعد إلغاء تنشيط دور أو انتهاء صلاحيه تنشيط الدور**</span><span class="sxs-lookup"><span data-stu-id="ad787-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="ad787-121">عند إلغاء تنشيط دور في أداره الهويات المميزة في Azure AD أو عند انتهاء صلاحيه فتره تنشيط دور ، قد يكون هناك تاخير حيث تستمر في الوصول.</span><span class="sxs-lookup"><span data-stu-id="ad787-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="ad787-122">إذا تم تاخير إلغاء التنشيط ، فاتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="ad787-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="ad787-123">إذا كنت تقوم بإلغاء تنشيط دور مسؤول Exchange أو إذا انتهت صلاحيه فتره تنشيط الدور ، وظهرت تاخيرا هاما قبل أزاله الأذونات ، فقم بفتح بطاقة دعم وأخبر مهندس الدعم لمساعدتك في الحصول علي البطاقة باستخدام فريق أداره الوصول المسموح به (بأم) داخل Office حول هذه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="ad787-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="ad787-124">إذا انتهت صلاحيه فتره التنشيط ، ولكنك لا تزال جلسة المستعرض مفتوحة ، فاغلق المستعرض.</span><span class="sxs-lookup"><span data-stu-id="ad787-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="ad787-125">يمكنك الاستمرار في استخدام الدور حتى تقوم بإغلاق جلسة العمل هذه.</span><span class="sxs-lookup"><span data-stu-id="ad787-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="ad787-126">هذه مشكله معروفه سنقوم بالاطلاع علي إصلاح محتمل لابطال كل جلسة بشكل فعال عند انتهاء صلاحيه التنشيط.</span><span class="sxs-lookup"><span data-stu-id="ad787-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="ad787-127">إذا كانت المهلة الخاصة بك مختلفه عن السيناريوين التاليين ، فالرجاء فتح تذكره دعم.</span><span class="sxs-lookup"><span data-stu-id="ad787-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
