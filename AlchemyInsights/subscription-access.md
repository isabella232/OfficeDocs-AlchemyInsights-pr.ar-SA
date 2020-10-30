---
title: الوصول إلى الاشتراك
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807157"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="371e9-102">تعذر تسجيل الدخول في Azure بسبب مشاكل في المستعرض (يتوقف المستعرض ، ولكنه لا يتم تحميله ، وغير ذلك.)</span><span class="sxs-lookup"><span data-stu-id="371e9-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="371e9-103">قد تتاثر بالانقطاع.</span><span class="sxs-lookup"><span data-stu-id="371e9-103">You might be impacted by an outage.</span></span> <span data-ttu-id="371e9-104">يرجى التحقق لمعرفه ما إذا كان هناك انقطاع مستمر: [حاله حماية Azure](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="371e9-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="371e9-105">يرجى تسجيل الخروج من كل جلسات عمل Azure النشطة.</span><span class="sxs-lookup"><span data-stu-id="371e9-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="371e9-106">أبدا تشغيل وضع خاص أو نافذه تصفح متخفي في مستعرض الويب.</span><span class="sxs-lookup"><span data-stu-id="371e9-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="371e9-107">يمكنك أيضا محاولة تحديث المستعرض ، واستخدام مستعرض آخر ، حذف ملفات تعريف الارتباط الخاصة بذاكره التخزين المؤقت إذا لم ينجح ذلك.</span><span class="sxs-lookup"><span data-stu-id="371e9-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="371e9-108">تعرف علي المزيد: [استكشاف مشاكل تسجيل الدخول وإصلاحها](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="371e9-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="371e9-109">**تعذر الوصول إلى الاشتراكات**</span><span class="sxs-lookup"><span data-stu-id="371e9-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="371e9-110">في [مدخل azure](https://portal.azure.com/)، تاكد من تحديد دليل azure الصحيح من الحساب في الجزء العلوي الأيسر.</span><span class="sxs-lookup"><span data-stu-id="371e9-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="371e9-111">في [مركز حسابات Azure](https://account.windowsazure.com/Subscriptions)، تاكد من ان الحساب المستخدم هو مسؤول الحساب.</span><span class="sxs-lookup"><span data-stu-id="371e9-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="371e9-112">معرفه المزيد: [استكشاف الأخطاء وإصلاحها لم يتم العثور علي اشتراكات](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="371e9-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="371e9-113">**تعذر الوصول إلى محفوظات الفوترة**</span><span class="sxs-lookup"><span data-stu-id="371e9-113">**Unable to access billing history**</span></span>

<span data-ttu-id="371e9-114">يحتاج مسؤول الحساب إلى التاكد من أضافه المستخدم الذي يقوم بالوصول إلى معلومات الفوترة في Azure Active directory كمستخدم ضيف: [أضافه مستخدم جديد أو حذفه](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="371e9-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="371e9-115">يجب ان يتم منح المستخدم الدور المسؤول العام: [تعيين الدور إلى المستخدمين](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="371e9-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="371e9-116">قم بنشر هذا المستخدم باستخدام نهج RBAC: [منح حق الوصول إلى الفوترة](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="371e9-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="371e9-117">**المستندات المستحسنة**</span><span class="sxs-lookup"><span data-stu-id="371e9-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="371e9-118">لا يمكنني تسجيل الدخول لأداره اشتراكك في Azure</span><span class="sxs-lookup"><span data-stu-id="371e9-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)