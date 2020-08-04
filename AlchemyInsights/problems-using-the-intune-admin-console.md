---
title: مشاكل في استخدام وحدة تحكم المسؤول Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554728"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="d52f3-102">مشاكل في استخدام وحدة تحكم المسؤول Intune</span><span class="sxs-lookup"><span data-stu-id="d52f3-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="d52f3-103">**"تم رفض الوصول" عند التنقل في مدخل مسؤول Intune.**</span><span class="sxs-lookup"><span data-stu-id="d52f3-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="d52f3-104">إذا كنت عضوًا في دور مخصص Intune، تأكد من تعيين ترخيص Intune أو مجموعة التنقل المؤسسي (EMS) إلى حسابك.</span><span class="sxs-lookup"><span data-stu-id="d52f3-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="d52f3-105">إذا كنت تستخدم إدارة التكوين لإدارة الأجهزة، تحقق من أنك لست جزءًا من مجموعة المستخدمين Intune لـ إدارة التكوين MDM.</span><span class="sxs-lookup"><span data-stu-id="d52f3-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="d52f3-106">تحقق من أنه تم تعيين الأذونات المناسبة للتحكم بالإدارة المستندة إلى الدور (RBAC) في النصل أدوار Intune.</span><span class="sxs-lookup"><span data-stu-id="d52f3-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="d52f3-107">تحقق من أن المجموعة المستخدمة ليست قائمة توزيع.</span><span class="sxs-lookup"><span data-stu-id="d52f3-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="d52f3-108">Intune في البوابة الإلكترونية أزور فقط يدعم حسابات المستخدمين التي تنتمي إلى مجموعات أمان Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d52f3-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="d52f3-109">راجع المجموعات الخاصة بك في البوابة Azure > مجموعات **إينتوني**  >  **Groups**، أو في بوابة Azure > Azure **Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="d52f3-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="d52f3-110">**المستخدم لديه الكثير من الأذونات لدور Intune المعينة**</span><span class="sxs-lookup"><span data-stu-id="d52f3-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="d52f3-111">تقديم المشورة للمستخدم للانتقال إلى **Intune**  >  **Intune الأدوار**بلدي  >  **أذونات**  >  **تصدير** لمراجعة الأذونات الممنوحة.</span><span class="sxs-lookup"><span data-stu-id="d52f3-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="d52f3-112">**لقد أضفت مجموعة نطاق إلى دور ما، ولكن لا يزال المستخدمون في هذا الدور يرون مستخدمين آخرين أو أجهزة أخرى.**</span><span class="sxs-lookup"><span data-stu-id="d52f3-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="d52f3-113">لا تقوم مجموعات النطاق بتصفية المستخدمين أو الأجهزة.</span><span class="sxs-lookup"><span data-stu-id="d52f3-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="d52f3-114">مجموعات النطاق:</span><span class="sxs-lookup"><span data-stu-id="d52f3-114">Scope groups:</span></span>

- <span data-ttu-id="d52f3-115">تحديد الأشخاص الذين يمكن للمستخدمين تعيين نُهج أو تطبيقات لهم.</span><span class="sxs-lookup"><span data-stu-id="d52f3-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="d52f3-116">السماح لمستخدمين معينين فقط بتشغيل المهام البعيدة على الأجهزة.</span><span class="sxs-lookup"><span data-stu-id="d52f3-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="d52f3-117">لمزيد من المعلومات حول مجموعات النطاق، راجع [التحكم بالوصول إلى الأدوار (RBAC) مع Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="d52f3-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="d52f3-118">**أضفت مستخدمًا إلى دور Intune ولكن لا يزال لديهم حق الوصول الكامل إلى وحدة تحكم Intune admin.**</span><span class="sxs-lookup"><span data-stu-id="d52f3-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="d52f3-119">انتقل إلى إينتوني > **المستخدمين** في البوابة الإلكترونية أزور وتحقق من أن المستخدم لم يتم تعيين إلى أي من الأدوار التالية في المدخل Azure:</span><span class="sxs-lookup"><span data-stu-id="d52f3-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="d52f3-120">مسؤول عمومي</span><span class="sxs-lookup"><span data-stu-id="d52f3-120">Global administrator</span></span>
- <span data-ttu-id="d52f3-121">مسؤول خدمة Intune</span><span class="sxs-lookup"><span data-stu-id="d52f3-121">Intune service administrator</span></span>
- <span data-ttu-id="d52f3-122">مسؤول SharePoint</span><span class="sxs-lookup"><span data-stu-id="d52f3-122">SharePoint administrator</span></span>

<span data-ttu-id="d52f3-123">لمزيد من المعلومات، راجع [التحكم في الوصول المستند إلى الدور (RBAC) مع Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="d52f3-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="d52f3-124">**مشاكل الوصول**</span><span class="sxs-lookup"><span data-stu-id="d52f3-124">**Access Issues**</span></span>

<span data-ttu-id="d52f3-125">لمزيد من المعلومات، راجع [لا يمكنك تسجيل الدخول إلى Office 365 أو Azure أو Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="d52f3-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>