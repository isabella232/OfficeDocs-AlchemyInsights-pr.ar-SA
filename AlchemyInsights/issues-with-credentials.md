---
title: مشاكل تتعلق باستخدام بيانات الاعتماد
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063578"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="b53ba-102">مشاكل تتعلق باستخدام بيانات الاعتماد</span><span class="sxs-lookup"><span data-stu-id="b53ba-102">Issues with credentials</span></span>

<span data-ttu-id="b53ba-103">يصف النظام الأساسي لهوية Microsoft وتدفق بيانات اعتماد عميل [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) كيفية برمجة بيانات اعتماد عميل OAuth 2.0 مباشرة مقابل منح التدفق.</span><span class="sxs-lookup"><span data-stu-id="b53ba-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="b53ba-104">**كيف يمكنني إدارة كلمة مرور التطبيق أو بيانات اعتماد الشهادة؟**</span><span class="sxs-lookup"><span data-stu-id="b53ba-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="b53ba-105">في Azure CLI، يمكنك استخدام بيانات اعتماد تطبيق [az ad](https://docs.microsoft.com/cli/azure/ad/app/credential) لحذف كلمة مرور التطبيق أو بيانات اعتماد الشهادة أو سردها أو إعادة تعيينها.</span><span class="sxs-lookup"><span data-stu-id="b53ba-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="b53ba-106">**كيف يمكن للمستخدمين إعادة تعيين كلمات المرور الخاصة بهم؟**</span><span class="sxs-lookup"><span data-stu-id="b53ba-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="b53ba-107">يحتاج المستخدمون [إلى التسجيل لإعادة تعيين](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) كلمة المرور للخدمة الذاتية قبل أن يستطيعوا إعادة تعيين كلمات المرور الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="b53ba-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="b53ba-108">بعد تسجيل المستخدم، يمكنه اتباع الإرشادات الواردة في هذه المقالة لإعادة تعيين كلمة المرور الخاصة به: إعادة تعيين كلمة مرور العمل [أو المدرسة.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)</span><span class="sxs-lookup"><span data-stu-id="b53ba-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="b53ba-109">**كيف يمكن للمستخدمين تغيير كلمات المرور الخاصة بهم؟**</span><span class="sxs-lookup"><span data-stu-id="b53ba-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="b53ba-110">يمكن للمستخدمين اتباع الخطوات في هذه المقالة لتغيير كلمات المرور الخاصة بهم: كيفية تغيير كلمة المرور الخاصة [بك.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="b53ba-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="b53ba-111">يمكنهم أيضا إدارة [كلمات مرور التطبيق للتحقق على خطوتين.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="b53ba-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="b53ba-112">**يحدث خطأ لدى المستخدم عند تغيير كلمة المرور أو إعادة تعيينها**</span><span class="sxs-lookup"><span data-stu-id="b53ba-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="b53ba-113">سيوفر هذا الارتباط معلومات حول المشاكل الشائعة التي قد تنشأ عندما يحاول المستخدم إعادة تعيين كلمة المرور الخاصة به: المشاكل الشائعة [وحلولها](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="b53ba-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="b53ba-114">**أواجه مشكلة في إعادة تعيين كلمة مرور المستخدم**</span><span class="sxs-lookup"><span data-stu-id="b53ba-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="b53ba-115">تأكد من أنك مفوض لإعادة تعيين كلمات المرور.</span><span class="sxs-lookup"><span data-stu-id="b53ba-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="b53ba-116">*يمكن للمسؤولين العامين وكلمة المرور والمستخدمين فقط إعادة تعيين كلمات مرور المستخدمين.*</span><span class="sxs-lookup"><span data-stu-id="b53ba-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="b53ba-117">يمكن للمسؤولين العامين أيضا إعادة تعيين كلمات مرور المسؤول المميز الأخرى.</span><span class="sxs-lookup"><span data-stu-id="b53ba-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="b53ba-118">تأكد من فهم متطلبات الترخيص:</span><span class="sxs-lookup"><span data-stu-id="b53ba-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="b53ba-119">يجب أن يكون لديك ترخيص واحد على الأقل تم تعيينه في مؤسستك:</span><span class="sxs-lookup"><span data-stu-id="b53ba-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="b53ba-120">**مستخدمو السحابة فقط** - أي SKU مدفوعة من Office 365 (O365) أو Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="b53ba-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="b53ba-121">المستخدمون في السحابة **و/أو** المحليون - Azure AD Premium P1 أو P2 أو Enterprise Mobility + Security (EMS) أو Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="b53ba-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="b53ba-122">لمعرفة المزيد حول متطلبات الترخيص، راجع متطلبات الترخيص لإعادة تعيين كلمة مرور الخدمة الذاتية ل [Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="b53ba-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="b53ba-123">لإعادة تعيين كلمة مرور مستخدم، ابحث عن المستخدم في Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b53ba-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="b53ba-124">بعد ذلك، على ريشة النظرة العامة لهذا المستخدم، انقر فوق الزر "إعادة تعيين كلمة المرور".</span><span class="sxs-lookup"><span data-stu-id="b53ba-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="b53ba-125">**زر إعادة تعيين كلمة المرور رمادي اللون**</span><span class="sxs-lookup"><span data-stu-id="b53ba-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="b53ba-126">أنت غير مفوض لإعادة **تعيين** كلمات مرور هذا المستخدم.</span><span class="sxs-lookup"><span data-stu-id="b53ba-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="b53ba-127">*يمكن للمسؤولين العامين وكلمة المرور والمستخدمين فقط إعادة تعيين كلمات مرور المستخدمين.*</span><span class="sxs-lookup"><span data-stu-id="b53ba-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="b53ba-128">يمكن للمسؤولين العامين أيضا إعادة تعيين كلمات مرور المسؤول المميز الأخرى.</span><span class="sxs-lookup"><span data-stu-id="b53ba-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="b53ba-129">**لا يمكنني رؤية ريشة إعادة تعيين كلمة المرور**</span><span class="sxs-lookup"><span data-stu-id="b53ba-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="b53ba-130">أنت غير مفوض لإعادة تعيين كلمات المرور.</span><span class="sxs-lookup"><span data-stu-id="b53ba-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="b53ba-131">*يمكن للمسؤولين العامين وكلمة المرور والمستخدمين فقط إعادة تعيين كلمات مرور المستخدمين.*</span><span class="sxs-lookup"><span data-stu-id="b53ba-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="b53ba-132">يمكن للمسؤولين العامين أيضا إعادة تعيين كلمات مرور المسؤول المميز الأخرى.</span><span class="sxs-lookup"><span data-stu-id="b53ba-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="b53ba-133">**لا يمكنني رؤية ريشة التكامل المحلي في إعادة تعيين كلمة المرور**</span><span class="sxs-lookup"><span data-stu-id="b53ba-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="b53ba-134">تظهر ريشة التكامل المحلي فقط في البيئات المختلطة ، مما يعني أنك تستخدم الكتابة بكلمة مرور لمعالجة كلمات مرور المستخدم المحلي.</span><span class="sxs-lookup"><span data-stu-id="b53ba-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="b53ba-135">لا ترى هذه الريشة في حالة:</span><span class="sxs-lookup"><span data-stu-id="b53ba-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="b53ba-136">أنت لا تستخدم إعادة كتابة كلمة المرور</span><span class="sxs-lookup"><span data-stu-id="b53ba-136">You are not using password writeback</span></span>
  - <span data-ttu-id="b53ba-137">توجد مشكلة في تثبيت/اتصال إعادة كتابة كلمة المرور</span><span class="sxs-lookup"><span data-stu-id="b53ba-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="b53ba-138">توجد مشكلة في تثبيت/اتصال Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="b53ba-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="b53ba-139">لمزيد من خطوات استكشاف الأخطاء وإصلاحها للمشاكل المتعلقة بكتابة كلمة المرور، راجع استكشاف الأخطاء [وإصلاحها في](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback) إعادة كتابة كلمة المرور</span><span class="sxs-lookup"><span data-stu-id="b53ba-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="b53ba-140">**لا أعرف كيفية إعادة تعيين كلمة مرور المستخدم**</span><span class="sxs-lookup"><span data-stu-id="b53ba-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="b53ba-141">سجل الدخول إلى مدخل Azure كمسؤول مناسب.</span><span class="sxs-lookup"><span data-stu-id="b53ba-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="b53ba-142">انتقل إلى **ريشة** المجموعات والمستخدمين، وحدد **"كل المستخدمين".**</span><span class="sxs-lookup"><span data-stu-id="b53ba-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="b53ba-143">حدد مستخدما من القائمة.</span><span class="sxs-lookup"><span data-stu-id="b53ba-143">Select a user from the list.</span></span>
4. <span data-ttu-id="b53ba-144">بالنسبة للمستخدم المحدد، حدد "نظرة **عامة"،** ثم في شريط الأوامر، حدد "إعادة تعيين كلمة **المرور".**</span><span class="sxs-lookup"><span data-stu-id="b53ba-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="b53ba-145">حدد الزر **"إعادة تعيين كلمة** المرور" واتبع الإرشادات التي تظهر على الشاشة.</span><span class="sxs-lookup"><span data-stu-id="b53ba-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="b53ba-146">عمليات إعادة التعيين التي يتم تنفيذها من خلال مدخل **Azure تدعم** إعادة كتابة كلمة المرور.</span><span class="sxs-lookup"><span data-stu-id="b53ba-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="b53ba-147">**أقوم بإعادة تعيين كلمة مرور مستخدم في الموقع المحلي من مدخل مسؤول Office 365 أو تطبيق Office 365 للجوال ولكن لا يزال المستخدم غير قادر على تسجيل الدخول**</span><span class="sxs-lookup"><span data-stu-id="b53ba-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="b53ba-148">الكتابة بكلمة مرور غير معتمدة في هذا المدخل.</span><span class="sxs-lookup"><span data-stu-id="b53ba-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="b53ba-149">أعد تعيين كلمة مرور المستخدم مرة أخرى في مدخل Azure.</span><span class="sxs-lookup"><span data-stu-id="b53ba-149">Reset the user's password again in the Azure portal.</span></span>
