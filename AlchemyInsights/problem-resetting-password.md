---
title: مشكلة في إعادة تعيين كلمة المرور
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692642"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="3b844-102">مشاكل في إعادة تعيين كلمة المرور</span><span class="sxs-lookup"><span data-stu-id="3b844-102">Problems resetting password</span></span>

<span data-ttu-id="3b844-103">فيما يلي بعض المشاكل التي قد تواجهها عند إعادة تعيين كلمة المرور والحلول الممكنة:</span><span class="sxs-lookup"><span data-stu-id="3b844-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="3b844-104">**أواجه مشكلة في إعادة تعيين كلمة المرور غير المتناولة في الفئات الأخرى**</span><span class="sxs-lookup"><span data-stu-id="3b844-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="3b844-105">تأكد من أنك مفوض لإعادة تعيين كلمات المرور.</span><span class="sxs-lookup"><span data-stu-id="3b844-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="3b844-106">يمكن للمسؤولين العامين وكلمة المرور والمستخدمين فقط إعادة تعيين كلمات مرور المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="3b844-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="3b844-107">يمكن للمسؤولين العامين أيضا إعادة تعيين كلمات مرور المسؤول المميز الأخرى.</span><span class="sxs-lookup"><span data-stu-id="3b844-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="3b844-108">تأكد من فهم متطلبات الترخيص:</span><span class="sxs-lookup"><span data-stu-id="3b844-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="3b844-109">يجب أن يكون لديك ترخيص واحد على الأقل تم تعيينه في مؤسستك</span><span class="sxs-lookup"><span data-stu-id="3b844-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="3b844-110">مستخدمو السحابة فقط - أي SKU مدفوعة من Office 365 (O365) أو Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="3b844-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="3b844-111">المستخدمون في السحابة و/أو المحليون - Azure AD Premium P1 أو P2 أو Enterprise Mobility + Security (EMS) أو Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="3b844-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="3b844-112">لقراءة المزيد حول متطلبات الترخيص، راجع متطلبات ترخيص المقالة لإعادة تعيين كلمة مرور الخدمة الذاتية ل [Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="3b844-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="3b844-113">**أواجه مشاكل في اختبار نهج إعادة تعيين كلمة المرور الذي حددته**</span><span class="sxs-lookup"><span data-stu-id="3b844-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="3b844-114">قد تستغرق السياسات المطبقة مؤخرا عدة دقائق لنسخها في كل مراكز البيانات ونقاط النهاية.</span><span class="sxs-lookup"><span data-stu-id="3b844-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="3b844-115">ستؤثر المسافة الفعلية من مركز البيانات أيضا على سرعة تطبيق التغييرات.</span><span class="sxs-lookup"><span data-stu-id="3b844-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="3b844-116">اختبار مع مستخدم، وليس مسؤول، وتجربته مع مجموعة صغيرة من المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="3b844-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="3b844-117">تنطبق السياسات التي تم تكوينها في مدخل Azure فقط على المستخدمين النهائيين، وليس المسؤولين.</span><span class="sxs-lookup"><span data-stu-id="3b844-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="3b844-118">تفرض Microsoft نهج إعادة تعيين كلمة مرور افتراضية وقوية ذات بوابتين لأي دور مسؤول Azure (على سبيل المثال: المسؤول العام، مسؤول المساعدة، مسؤول كلمة المرور، إلخ.)</span><span class="sxs-lookup"><span data-stu-id="3b844-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="3b844-119">تعرف على المزيد [حول سياسات المسؤولين.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="3b844-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="3b844-120">**أريد نشر إعادة تعيين كلمة المرور ولكن لا أريد جعل المستخدمين يسجلون معلومات أمان إضافية**</span><span class="sxs-lookup"><span data-stu-id="3b844-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="3b844-121">ملء البيانات مسبقا للمستخدمين بحيث لا يحتاجوا إلى ذلك!</span><span class="sxs-lookup"><span data-stu-id="3b844-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="3b844-122">- كمسؤول، يمكنك تعيين خصائص الهاتف والبريد الإلكتروني للمستخدمين قبل طرح إعادة تعيين كلمة المرور إلى مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="3b844-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="3b844-123">يمكنك القيام بذلك باستخدام API أو PowerShell أو Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="3b844-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="3b844-124">مزيد من المعلومات هنا:</span><span class="sxs-lookup"><span data-stu-id="3b844-124">More information here:</span></span>
- [<span data-ttu-id="3b844-125">نشر إعادة تعيين كلمة المرور دون مطالبة المستخدمين بالتسجيل</span><span class="sxs-lookup"><span data-stu-id="3b844-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="3b844-126">البيانات التي تستخدمها إعادة تعيين كلمة المرور</span><span class="sxs-lookup"><span data-stu-id="3b844-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="3b844-127">**زر إعادة تعيين كلمة المرور رمادي اللون**</span><span class="sxs-lookup"><span data-stu-id="3b844-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="3b844-128">أنت غير مفوض لإعادة تعيين كلمات مرور هذا المستخدم.</span><span class="sxs-lookup"><span data-stu-id="3b844-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="3b844-129">يمكن للمسؤولين العامين وكلمة المرور والمستخدمين فقط إعادة تعيين كلمات مرور المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="3b844-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="3b844-130">يمكن للمسؤولين العامين أيضا إعادة تعيين كلمات مرور المسؤول المميز الأخرى.</span><span class="sxs-lookup"><span data-stu-id="3b844-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="3b844-131">**لا يمكنني رؤية ريشة إعادة تعيين كلمة المرور**</span><span class="sxs-lookup"><span data-stu-id="3b844-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="3b844-132">أنت غير مفوض لإعادة تعيين كلمات المرور.</span><span class="sxs-lookup"><span data-stu-id="3b844-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="3b844-133">يمكن للمسؤولين العامين وكلمة المرور والمستخدمين فقط إعادة تعيين كلمات مرور المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="3b844-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="3b844-134">يمكن للمسؤولين العامين أيضا إعادة تعيين كلمات مرور المسؤول المميز الأخرى.</span><span class="sxs-lookup"><span data-stu-id="3b844-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="3b844-135">**لا يمكنني رؤية ريشة التكامل المحلي في إعادة تعيين كلمة المرور**</span><span class="sxs-lookup"><span data-stu-id="3b844-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="3b844-136">تظهر ريشة التكامل المحلي فقط في البيئات المختلطة ، مما يعني أنك تستخدم الكتابة بكلمة مرور لمعالجة كلمات مرور المستخدم المحلي.</span><span class="sxs-lookup"><span data-stu-id="3b844-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="3b844-137">لا ترى هذه الريشة في حالة:</span><span class="sxs-lookup"><span data-stu-id="3b844-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="3b844-138">أنت لا تستخدم إعادة كتابة كلمة المرور</span><span class="sxs-lookup"><span data-stu-id="3b844-138">You are not using password writeback</span></span>
    - <span data-ttu-id="3b844-139">توجد مشكلة في تثبيت/اتصال إعادة كتابة كلمة المرور</span><span class="sxs-lookup"><span data-stu-id="3b844-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="3b844-140">توجد مشكلة في تثبيت/اتصال Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="3b844-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="3b844-141">للحصول على مزيد من خطوات استكشاف الأخطاء وإصلاحها للمشاكل المتعلقة بكتابة كلمة المرور، راجع القسم "استكشاف الأخطاء في إعادة كتابة كلمة [المرور وإصلاحها"](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="3b844-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="3b844-142">**لا أعرف كيفية إعادة تعيين كلمة مرور المستخدم**</span><span class="sxs-lookup"><span data-stu-id="3b844-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="3b844-143">سجل الدخول إلى مدخل Azure كمسؤول مناسب.</span><span class="sxs-lookup"><span data-stu-id="3b844-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="3b844-144">انتقل إلى ريشة المجموعات والمستخدمين، وحدد **"كل المستخدمين".**</span><span class="sxs-lookup"><span data-stu-id="3b844-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="3b844-145">حدد مستخدما من القائمة.</span><span class="sxs-lookup"><span data-stu-id="3b844-145">Select a user from the list.</span></span>
1. <span data-ttu-id="3b844-146">بالنسبة للمستخدم المحدد، حدد "نظرة **عامة"،** ثم في شريط الأوامر، انقر فوق "إعادة تعيين كلمة **المرور".**</span><span class="sxs-lookup"><span data-stu-id="3b844-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="3b844-147">اتبع الإرشادات التي تظهر على الشاشة.</span><span class="sxs-lookup"><span data-stu-id="3b844-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="3b844-148">عمليات إعادة التعيين التي يتم تنفيذها من خلال مدخل Azure تدعم إعادة كتابة كلمة المرور.</span><span class="sxs-lookup"><span data-stu-id="3b844-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="3b844-149">**أقوم بإعادة تعيين كلمة مرور مستخدم في الموقع المحلي من مدخل مسؤول Office 365 أو تطبيق Office 365 للجوال ولكن لا يزال المستخدم غير قادر على تسجيل الدخول**</span><span class="sxs-lookup"><span data-stu-id="3b844-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="3b844-150">الكتابة بكلمة مرور غير معتمدة في هذا المدخل.</span><span class="sxs-lookup"><span data-stu-id="3b844-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="3b844-151">إعادة تعيين كلمة مرور المستخدم مرة أخرى في مدخل Azure - portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="3b844-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

