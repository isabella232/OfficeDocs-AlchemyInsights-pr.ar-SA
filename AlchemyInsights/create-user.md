---
title: إنشاء مستخدم
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569698"
---
# <a name="create-user"></a><span data-ttu-id="28a04-102">إنشاء مستخدم</span><span class="sxs-lookup"><span data-stu-id="28a04-102">Create user</span></span>

<span data-ttu-id="28a04-103">**الإعلان:**</span><span class="sxs-lookup"><span data-stu-id="28a04-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="28a04-104">إهمال دعم تسجيل الدخول إلى WebView من Google بدءا من 4 يناير [2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span><span class="sxs-lookup"><span data-stu-id="28a04-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="28a04-105">اختبر ما إذا كانت تطبيقاتك قد تتأثر باتباع إرشادات [Google](https://go.microsoft.com/fwlink/?linkid=2157323) حول اختبار التوافق.</span><span class="sxs-lookup"><span data-stu-id="28a04-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="28a04-106">تأكد من استخدام عرض ويب للنظام أو مستعرض النظام عند تسجيل الدخول إلى المستخدمين باستخدام حسابات Google للمستهلكين.</span><span class="sxs-lookup"><span data-stu-id="28a04-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="28a04-107">لمزيد من المعلومات، راجع مشاكل تسجيل الدخول إلى [التطبيق (التطبيقات) باستخدام مستعرض Chrome فقط](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span><span class="sxs-lookup"><span data-stu-id="28a04-107">For more information, see [Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="28a04-108">**لا يمكنني إنشاء مستخدم جديد في دليل Azure AD**</span><span class="sxs-lookup"><span data-stu-id="28a04-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="28a04-109">تأكد من أنك م مخولا لإنشاء مستخدم قياسي جديد.</span><span class="sxs-lookup"><span data-stu-id="28a04-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="28a04-110">يمكن فقط لدور المسؤول العام أو مسؤول المستخدم في Azure Active Directory (AD) إنشاء مستخدم قياسي جديد.</span><span class="sxs-lookup"><span data-stu-id="28a04-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="28a04-111">إذا لم تكن في أحد هذه الأدوار، فاطلب من المسؤول إضافتك إلى أحد هذه الأدوار أو إنشاء حساب مستخدم جديد لك.</span><span class="sxs-lookup"><span data-stu-id="28a04-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="28a04-112">تأكد من أن اسم المستخدم في مجال تم التحقق منه في Azure AD.</span><span class="sxs-lookup"><span data-stu-id="28a04-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="28a04-113">إذا لم يكن لديك أي أسماء مجالات مخصصة متحقق منها في Azure AD، يمكنك استخدام مجال Azure AD الأولي، الذي ينتهي ب \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="28a04-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="28a04-114">تأكد من أن اسم المستخدم في مجال غير متكاتف مع Azure AD من AD الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="28a04-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="28a04-115">لا يمكن إضافة المستخدمين في السحابة مع أسماء المجالات التي يتم تدائمها من الأسماء في الموقع.</span><span class="sxs-lookup"><span data-stu-id="28a04-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="28a04-116">تأكد من عدم وجود اسم مستخدم أو جهة اتصال أخرى تريد تعيينه إلى المستخدم الجديد.</span><span class="sxs-lookup"><span data-stu-id="28a04-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="28a04-117">يجب أن تكون أسماء المستخدمين فريدة عبر Azure AD.</span><span class="sxs-lookup"><span data-stu-id="28a04-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="28a04-118">راجع [أدوار Azure AD والمسؤولين](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) ل Azure AD.</span><span class="sxs-lookup"><span data-stu-id="28a04-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="28a04-119">راجع [أسماء مجالات](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="28a04-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="28a04-120">راجع [سجلات التدقيق](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) لرؤية معلومات أكثر تفصيلا حول مستخدم تم إنشاؤه أو حذفه مؤخرا مثل الشخص الذي قام بتنفيذ الإجراء ومتى.</span><span class="sxs-lookup"><span data-stu-id="28a04-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="28a04-121">لمزيد من المعلومات حول إضافة مستخدمين جدد، راجع استخدام مدخل Azure لإنشاء مستخدم [جديد في Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="28a04-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="28a04-122">[أدوار Azure AD الإدارية](/azure/active-directory/active-directory-assign-admin-roles): أذونات دور المسؤول في Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="28a04-122">[Azure AD administrative roles](/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="28a04-123">يمكنك أيضا [استخدام Azure AD PowerShell لإنشاء مستخدم جديد](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span><span class="sxs-lookup"><span data-stu-id="28a04-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
