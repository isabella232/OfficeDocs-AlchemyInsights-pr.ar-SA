---
title: مشاكل إدارة المستخدمين
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034815"
---
# <a name="user-management-issues"></a><span data-ttu-id="8aab1-102">مشاكل إدارة المستخدمين</span><span class="sxs-lookup"><span data-stu-id="8aab1-102">User management issues</span></span>

<span data-ttu-id="8aab1-103">**ماذا يحدث للمستخدمين المعينين حاليا للتطبيق إذا قمت بتعطيل الخاصية "تعيين المستخدم مطلوب" (قم بتعيين هذه الخاصية إلى لا)؟**</span><span class="sxs-lookup"><span data-stu-id="8aab1-103">**What happens to current assigned users to the application if I disable the property ‘User assignment required’ (set this property to No)?**</span></span>

<span data-ttu-id="8aab1-104">لا يؤثر **تعطيل تعيين** المستخدم المطلوب على المستخدمين المعينين حاليا.</span><span class="sxs-lookup"><span data-stu-id="8aab1-104">Disabling **User assignment required** does NOT affect the currently assigned users.</span></span> <span data-ttu-id="8aab1-105">سيسمح تعطيل هذه الخاصية فقط لجميع المستخدمين بالوصول إلى التطبيق.</span><span class="sxs-lookup"><span data-stu-id="8aab1-105">Disabling this property will only allow all users to access the application.</span></span> <span data-ttu-id="8aab1-106">وسيبقى جميع المستخدمين المدرجين والمستخدمين المعينين إلى مجموعات في التطبيق صالحين.</span><span class="sxs-lookup"><span data-stu-id="8aab1-106">All the listed users and those users assigned to groups in the application will still be valid.</span></span>

- <span data-ttu-id="8aab1-107">لتقييد تطبيقك إلى مجموعة معينة من المستخدمين، راجع - تقييد تطبيق Azure AD إلى مجموعة من المستخدمين - النظام الأساسي [لهوية Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span><span class="sxs-lookup"><span data-stu-id="8aab1-107">To restrict your app to specific set of users, see - [Restrict Azure AD app to a set of users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span></span>
- <span data-ttu-id="8aab1-108">لتعيين المستخدمين والمجموعات، لتطبيقات المؤسسة في Azure Active Directory (Azure AD)، إما من داخل مدخل Azure أو باستخدام PowerShell، راجع إدارة تعيين المستخدم لتطبيق في [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span><span class="sxs-lookup"><span data-stu-id="8aab1-108">To assign users and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span>
- <span data-ttu-id="8aab1-109">لتفويض أذونات إنشاء التطبيق وإدارته، راجع تفويض أذونات مسؤول إدارة التطبيقات [- Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span><span class="sxs-lookup"><span data-stu-id="8aab1-109">To delegate Application creation and management permissions, see [Delegate application management administrator permissions - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span></span>
- <span data-ttu-id="8aab1-110">**إخفاء تطبيقات المؤسسة المحددة عن المستخدمين** - استخدم الخطوات التالية لإخفاء جميع تطبيقات Microsoft 365 من لوحة **MyApps.**</span><span class="sxs-lookup"><span data-stu-id="8aab1-110">**Hide specific enterprise apps from users** - Use the following steps to hide all Microsoft 365 apps from the **MyApps** panel.</span></span> <span data-ttu-id="8aab1-111">وستبقى التطبيقات مرئية في مدخل Office 365.</span><span class="sxs-lookup"><span data-stu-id="8aab1-111">The apps will still be visible in the Office 365 portal.</span></span>

 1. <span data-ttu-id="8aab1-112">سجل الدخول إلى مدخل Azure كمسؤول عام للدراج.</span><span class="sxs-lookup"><span data-stu-id="8aab1-112">Sign-in to the Azure portal as a global administrator for your directory.</span></span> 
 2. <span data-ttu-id="8aab1-113">حدد **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="8aab1-113">Select **Azure Active Directory**.</span></span> 
 3. <span data-ttu-id="8aab1-114">حدد **المستخدمون**.</span><span class="sxs-lookup"><span data-stu-id="8aab1-114">Select **Users**.</span></span> 
 4. <span data-ttu-id="8aab1-115">حدد **إعدادات المستخدم**.</span><span class="sxs-lookup"><span data-stu-id="8aab1-115">Select **User settings**.</span></span> 
 5. <span data-ttu-id="8aab1-116">ضمن **تطبيقات المؤسسة،** انقر فوق **إدارة كيفية تشغيل المستخدمين النهائيين للتطبيقات وعرضها**.</span><span class="sxs-lookup"><span data-stu-id="8aab1-116">Under **Enterprise applications**, click **Manage how end users launch and view their applications**.</span></span> 
 6. <span data-ttu-id="8aab1-117">بالنسبة **للمستخدمين، يمكنهم رؤية تطبيقات Office 365 فقط في مدخل Office 365،** انقر فوق **نعم**.</span><span class="sxs-lookup"><span data-stu-id="8aab1-117">For **Users can only see Office 365 apps in the Office 365 portal**, click **Yes**.</span></span> 
 7. <span data-ttu-id="8aab1-118">انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="8aab1-118">Click **Save**.</span></span> 
 8. <span data-ttu-id="8aab1-119">لمزيد من التفاصيل، راجع إخفاء تطبيق Enterprise من تجربة المستخدم [في Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span><span class="sxs-lookup"><span data-stu-id="8aab1-119">For more details, see [Hide an Enterprise application from user's experience in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span></span>

- <span data-ttu-id="8aab1-120">إذا كنت تعرض تطبيق "برامج" كخدمة (SaaS) للعديد من المؤسسات، يمكنك تكوين تطبيقك لقبول تسجيل الدخول من أي مستأجر Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="8aab1-120">If you offer a Software as a Service (SaaS) app to many organizations, you can configure your app to accept sign-ins from any Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="8aab1-121">يسمى هذا التكوين "جعل تطبيقك متعدد المستأجرين".</span><span class="sxs-lookup"><span data-stu-id="8aab1-121">This configuration is called "making your application multi-tenant".</span></span> <span data-ttu-id="8aab1-122">وسيتمكن المستخدمون في أي مستأجر Azure AD من تسجيل الدخول إلى تطبيقك بعد الموافقة على استخدام حسابهم مع تطبيقك.</span><span class="sxs-lookup"><span data-stu-id="8aab1-122">Users in any Azure AD tenant will be able to sign-in to your app after consenting to use their account with your app.</span></span> <span data-ttu-id="8aab1-123">لمزيد من المعلومات، راجع إنشاء التطبيقات التي تقوم تسجيل الدخول إلى [مستخدمي Azure AD - النظام الأساسي لهوية Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span><span class="sxs-lookup"><span data-stu-id="8aab1-123">For more information, see [Build apps that sign in Azure AD users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span></span>

- <span data-ttu-id="8aab1-124">**كيف يمكن للمستخدم الوصول إلى التطبيق بمجرد تعيينه للتطبيق؟**</span><span class="sxs-lookup"><span data-stu-id="8aab1-124">**How can an end user access the application once he/she is assigned to the application?**</span></span>

<span data-ttu-id="8aab1-125">يحتوي كل تطبيق في شفرة تطبيق Enterprise على ارتباط يمكن للمستخدمين الوصول إليه.</span><span class="sxs-lookup"><span data-stu-id="8aab1-125">Each app in Enterprise application blade has a link for end users to access.</span></span> <span data-ttu-id="8aab1-126">يمكن للمستخدمين أيضا الوصول إلى التطبيق من خلال **مدخل Myapps** بطريقة سهلة.</span><span class="sxs-lookup"><span data-stu-id="8aab1-126">Users can also access the app through **Myapps** portal in an easy way.</span></span>

- <span data-ttu-id="8aab1-127">**هل تريد معرفة التطبيقات ونوع التطبيقات التي يستخدمها المستخدمون؟**</span><span class="sxs-lookup"><span data-stu-id="8aab1-127">**Want to know which applications and type of applications are being used by users?**</span></span>

<span data-ttu-id="8aab1-128">يمكنك تنزيل تقارير تسجيل الدخول خلال آخر 30 يوما من portal.azure.com > **Azure Active directory**> Signins> تقارير التنزيل.</span><span class="sxs-lookup"><span data-stu-id="8aab1-128">You can download sign-in reports for the last 30 days from **portal.azure.com > Azure Active directory> Signins> download reports**.</span></span>

- <span data-ttu-id="8aab1-129">تعرف على كيفية منح موافقة المسؤول على نطاق [المستأجر لتطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) وتكوين كيفية موافقة [المستخدمين النهائيين على التطبيقات.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)</span><span class="sxs-lookup"><span data-stu-id="8aab1-129">Learn how to [Grant tenant wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) and [Configure how end users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span></span>

- <span data-ttu-id="8aab1-130">فهم [كيفية عمل الموافقة](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) وإدارة الموافقة على [التطبيقات](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span><span class="sxs-lookup"><span data-stu-id="8aab1-130">Understand [how consent works](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) and [Manage consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span></span>


