---
title: كيفيه أضافه المسؤولين وأدارههم
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
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755426"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="77e00-102">كيفيه أضافه المسؤولين وأدارههم</span><span class="sxs-lookup"><span data-stu-id="77e00-102">How to add and manage admins</span></span>

<span data-ttu-id="77e00-103">بالاستناد إلى وصف المشكلة ، لقد عثرنا علي حل لك.</span><span class="sxs-lookup"><span data-stu-id="77e00-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="77e00-104">يستطيع معظم العملاء حل مشكلتهم بنفسهم بعد متابعه الوثائق الخاصة بنا.</span><span class="sxs-lookup"><span data-stu-id="77e00-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="77e00-105">لأداره حساب الفوترة لاتفاقيه عملاء Microsoft (MCA) ، يمكنك استخدام ادوار مختلفه باستخدام مستوي الوصول المطلوب.</span><span class="sxs-lookup"><span data-stu-id="77e00-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="77e00-106">هذه الأدوار بالاضافه إلى ادوار خدمه Azure المضمنة التي تساعدك علي التحكم بالموارد.</span><span class="sxs-lookup"><span data-stu-id="77e00-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="77e00-107">**لأضافه ادوار الفوترة في مدخل Azure:**</span><span class="sxs-lookup"><span data-stu-id="77e00-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="77e00-108">سجل دخولك إلى [مدخل Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="77e00-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="77e00-109">البحث عن *أداره التكاليف + الفوترة*.</span><span class="sxs-lookup"><span data-stu-id="77e00-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="77e00-110">حدد التحكم بالوصول (أيام) في نطاق مثل حساب الفوترة أو ملف تعريف الفوترة أو مقطع الفاتورة حيث تريد منح حق الوصول.</span><span class="sxs-lookup"><span data-stu-id="77e00-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="77e00-111">تسرد صفحه التحكم بالوصول (أيام) المستخدمين والمجموعات التي تم تعيينها لكل دور لهذا النطاق.</span><span class="sxs-lookup"><span data-stu-id="77e00-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="77e00-112">لمنح حق الوصول إلى مستخدم ، حدد **أضافه** من اعلي الصفحة.</span><span class="sxs-lookup"><span data-stu-id="77e00-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="77e00-113">في القائمة المنسدلة *الدور* ، حدد دورا.</span><span class="sxs-lookup"><span data-stu-id="77e00-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="77e00-114">ادخل عنوان البريد الكتروني الخاص بالمستخدم الذي تريد منحه حق الوصول.</span><span class="sxs-lookup"><span data-stu-id="77e00-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="77e00-115">حدد **حفظ** لتعيين الدور.</span><span class="sxs-lookup"><span data-stu-id="77e00-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="77e00-116">لأزاله حق الوصول لمستخدم ما ، حدد المستخدم الذي يحتوي علي تعيين الدور الذي تريد ازالته.</span><span class="sxs-lookup"><span data-stu-id="77e00-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="77e00-117">حدد **أزاله**.</span><span class="sxs-lookup"><span data-stu-id="77e00-117">Select **Remove**.</span></span>

<span data-ttu-id="77e00-118">**المستندات المستحسنة**</span><span class="sxs-lookup"><span data-stu-id="77e00-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="77e00-119">تعريفات ادوار الفوترة</span><span class="sxs-lookup"><span data-stu-id="77e00-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="77e00-120">ادوار حساب الفوترة ومهامه</span><span class="sxs-lookup"><span data-stu-id="77e00-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="77e00-121">بدء استخدام حساب الفوترة في MCA</span><span class="sxs-lookup"><span data-stu-id="77e00-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="77e00-122">التحقق من الوصول إلى اتفاقيه عملاء Microsoft</span><span class="sxs-lookup"><span data-stu-id="77e00-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
