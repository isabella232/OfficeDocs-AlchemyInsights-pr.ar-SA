---
title: كيفيه أضافه المسؤولين وأدارهم-FL/كل
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
- "9004114"
- "7424"
ms.openlocfilehash: f5791cb12e565cb04f7ac6bc9bb401fcca3e4e9e
ms.sourcegitcommit: dd9eb38bf9403de29f46c844cb64bc1d4c515afc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2020
ms.locfileid: "49691927"
---
# <a name="how-to-add-and-manage-admins---mca-flcl"></a><span data-ttu-id="dad8c-102">كيفيه أضافه المسؤولين وأدارهم-FL/كل</span><span class="sxs-lookup"><span data-stu-id="dad8c-102">How to add and manage admins - MCA FL/CL</span></span>

<span data-ttu-id="dad8c-103">لأداره حساب الفوترة لاتفاقيه عملاء Microsoft (MCA) ، يمكنك استخدام ادوار مختلفه باستخدام مستوي الوصول المطلوب.</span><span class="sxs-lookup"><span data-stu-id="dad8c-103">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="dad8c-104">هذه الأدوار بالاضافه إلى ادوار خدمه Azure المضمنة التي تساعدك علي التحكم بالموارد.</span><span class="sxs-lookup"><span data-stu-id="dad8c-104">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="dad8c-105">**لأضافه ادوار الفوترة في مدخل Azure:**</span><span class="sxs-lookup"><span data-stu-id="dad8c-105">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="dad8c-106">سجل دخولك إلى [مدخل Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="dad8c-106">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="dad8c-107">البحث عن *أداره التكاليف + الفوترة*.</span><span class="sxs-lookup"><span data-stu-id="dad8c-107">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="dad8c-108">حدد التحكم بالوصول (أيام) في نطاق مثل حساب الفوترة أو ملف تعريف الفوترة أو مقطع الفاتورة حيث تريد منح حق الوصول.</span><span class="sxs-lookup"><span data-stu-id="dad8c-108">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="dad8c-109">تسرد صفحه التحكم بالوصول (أيام) المستخدمين والمجموعات التي تم تعيينها لكل دور لهذا النطاق.</span><span class="sxs-lookup"><span data-stu-id="dad8c-109">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="dad8c-110">لمنح حق الوصول إلى مستخدم ، حدد **أضافه** من اعلي الصفحة.</span><span class="sxs-lookup"><span data-stu-id="dad8c-110">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="dad8c-111">في القائمة المنسدلة *الدور* ، حدد دورا.</span><span class="sxs-lookup"><span data-stu-id="dad8c-111">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="dad8c-112">ادخل عنوان البريد الكتروني الخاص بالمستخدم الذي تريد منحه حق الوصول.</span><span class="sxs-lookup"><span data-stu-id="dad8c-112">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="dad8c-113">حدد **حفظ** لتعيين الدور.</span><span class="sxs-lookup"><span data-stu-id="dad8c-113">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="dad8c-114">لأزاله حق الوصول لمستخدم ما ، حدد المستخدم الذي يحتوي علي تعيين الدور الذي تريد ازالته.</span><span class="sxs-lookup"><span data-stu-id="dad8c-114">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="dad8c-115">حدد **أزاله**.</span><span class="sxs-lookup"><span data-stu-id="dad8c-115">Select **Remove**.</span></span>

<span data-ttu-id="dad8c-116">**المستندات المستحسنة**</span><span class="sxs-lookup"><span data-stu-id="dad8c-116">**Recommended Documents**</span></span>

- [<span data-ttu-id="dad8c-117">تعريفات ادوار الفوترة</span><span class="sxs-lookup"><span data-stu-id="dad8c-117">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="dad8c-118">ادوار حساب الفوترة ومهامه</span><span class="sxs-lookup"><span data-stu-id="dad8c-118">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="dad8c-119">بدء استخدام حساب الفوترة في MCA</span><span class="sxs-lookup"><span data-stu-id="dad8c-119">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="dad8c-120">التحقق من الوصول إلى اتفاقيه عملاء Microsoft</span><span class="sxs-lookup"><span data-stu-id="dad8c-120">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
