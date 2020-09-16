---
title: المشاكل المتعلقة باستخدام وحده تحكم مسؤول Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728274"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="37001-102">المشاكل المتعلقة باستخدام وحده تحكم مسؤول Intune</span><span class="sxs-lookup"><span data-stu-id="37001-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="37001-103">**"تم رفض الوصول" عند التنقل في مدخل مسؤول Intune.**</span><span class="sxs-lookup"><span data-stu-id="37001-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="37001-104">إذا كنت عضوا في دور Intune مخصص ، فتاكد من انه تم تعيين ترخيص المجموعة "الخاصة ب Intune" (EMS) لحسابك.</span><span class="sxs-lookup"><span data-stu-id="37001-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="37001-105">إذا كنت تستخدم أداره التكوين لأداره الاجهزه ، فتحقق من انك لست جزءا من مجموعه مستخدمي Intune لأداره التكوين MDM.</span><span class="sxs-lookup"><span data-stu-id="37001-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="37001-106">تاكد من انك قمت بتعيين أذونات التحكم المناسبة المستندة إلى الدور (RBAC) في ريش ادوار Intune.</span><span class="sxs-lookup"><span data-stu-id="37001-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="37001-107">تاكد من ان المجموعة المستخدمة ليست قائمه توزيع.</span><span class="sxs-lookup"><span data-stu-id="37001-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="37001-108">يعتمد Intune في مدخل Azure حسابات المستخدمين الذين ينتمون إلى مجموعات أمان Azure Active directory فقط.</span><span class="sxs-lookup"><span data-stu-id="37001-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="37001-109">قم بمراجعه مجموعاتك في مجموعات azure portal > **Intune**  >  **Groups**، أو في azure portal > **Azure active**directory.</span><span class="sxs-lookup"><span data-stu-id="37001-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="37001-110">**يملك المستخدم العديد من الأذونات لدور Intune المعين**</span><span class="sxs-lookup"><span data-stu-id="37001-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="37001-111">قم باعلام المستخدم بالانتقال إلى ادوار **intune**  >  **intune**  >  **الخاصة بي**  >  **Export** لمراجعه الأذونات الممنوحة.</span><span class="sxs-lookup"><span data-stu-id="37001-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="37001-112">**لقد أضفت مجموعه نطاقات إلى أحد الأدوار ، ولكن ما زال بإمكان المستخدمين في هذا الدور رؤية المستخدمين أو الاجهزه الأخرى.**</span><span class="sxs-lookup"><span data-stu-id="37001-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="37001-113">لا تقوم مجموعات النطاقات بتصفية المستخدمين أو الاجهزه.</span><span class="sxs-lookup"><span data-stu-id="37001-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="37001-114">مجموعات النطاقات:</span><span class="sxs-lookup"><span data-stu-id="37001-114">Scope groups:</span></span>

- <span data-ttu-id="37001-115">تحديد الأشخاص الذين يمكنهم تعيين النهج أو التطبيقات اليهم.</span><span class="sxs-lookup"><span data-stu-id="37001-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="37001-116">السماح لمستخدمين محددين فقط بتشغيل المهام البعيدة علي الاجهزه.</span><span class="sxs-lookup"><span data-stu-id="37001-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="37001-117">للحصول علي مزيد من المعلومات حول مجموعات النطاقات ، راجع  [التحكم في الوصول القائم علي الدور (RBAC) باستخدام Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="37001-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="37001-118">**لقد أضفت مستخدما إلى دور Intune ولكنه ما زال لديه حق الوصول الكامل إلى وحده تحكم مسؤول Intune.**</span><span class="sxs-lookup"><span data-stu-id="37001-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="37001-119">انتقل إلى Intune > **المستخدمين** في مدخل Azure وتحقق من عدم تعيين المستخدم إلى اي من الأدوار التالية في مدخل azure:</span><span class="sxs-lookup"><span data-stu-id="37001-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="37001-120">المسؤول العام</span><span class="sxs-lookup"><span data-stu-id="37001-120">Global administrator</span></span>
- <span data-ttu-id="37001-121">مسؤول خدمه Intune</span><span class="sxs-lookup"><span data-stu-id="37001-121">Intune service administrator</span></span>
- <span data-ttu-id="37001-122">مسؤول SharePoint</span><span class="sxs-lookup"><span data-stu-id="37001-122">SharePoint administrator</span></span>

<span data-ttu-id="37001-123">للحصول علي مزيد من المعلومات ، راجع [التحكم في الوصول القائم علي الأدوار (RBAC) باستخدام Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="37001-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="37001-124">**مشاكل في الوصول**</span><span class="sxs-lookup"><span data-stu-id="37001-124">**Access Issues**</span></span>

<span data-ttu-id="37001-125">لمزيد من المعلومات ، راجع [لا يمكنك تسجيل الدخول إلى Office 365 أو Azure أو Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="37001-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>