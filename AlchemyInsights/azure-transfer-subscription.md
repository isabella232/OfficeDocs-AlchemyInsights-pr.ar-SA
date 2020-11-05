---
title: نقل ملكيه الفوترة في Azure
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/03/2020
ms.locfileid: "48921989"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="1ac3d-102">نقل ملكيه الفوترة في Azure</span><span class="sxs-lookup"><span data-stu-id="1ac3d-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="1ac3d-103">قم بتسجيل الدخول إلى [مدخل Azure](https://portal.azure.com/) كمسؤول لحساب الفوترة الذي يحتوي علي الاشتراك الذي تريد نقله.</span><span class="sxs-lookup"><span data-stu-id="1ac3d-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="1ac3d-104">إذا لم تكن متاكدا مما إذا كنت أنت والمسؤول ، أو إذا كنت بحاجه إلى تحديد الأشخاص ، فراجع التعرف علي [مسؤول فوتره الحساب](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="1ac3d-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="1ac3d-105">البحث في **أداره التكاليف + الفوترة**.</span><span class="sxs-lookup"><span data-stu-id="1ac3d-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="1ac3d-106">حدد **الاشتراكات** من الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="1ac3d-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="1ac3d-107">استنادا إلى access ، قد تحتاج إلى تحديد نطاق تحرير فواتير **والاشتراكات** أو **اشتراكات Azure**.</span><span class="sxs-lookup"><span data-stu-id="1ac3d-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="1ac3d-108">تحديد **نقل ملكيه الفوترة** للاشتراك الذي تريد نقله</span><span class="sxs-lookup"><span data-stu-id="1ac3d-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="1ac3d-109">ادخل عنوان البريد الكتروني للمستخدم الذي يكون مسؤول الفوترة الخاص بالحساب الذي سيكون مالكه الجديد للاشتراك ، ثم حدد **إرسال طلب تحويل**</span><span class="sxs-lookup"><span data-stu-id="1ac3d-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="1ac3d-110">يحصل المستخدم علي رسالة بريد الكتروني تتضمن إرشادات لمراجعه طلب النقل.</span><span class="sxs-lookup"><span data-stu-id="1ac3d-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="1ac3d-111">للموافقة علي طلب النقل ، يقوم المستخدم بتحديد الارتباط في البريد الكتروني واتباع الإرشادات.</span><span class="sxs-lookup"><span data-stu-id="1ac3d-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="1ac3d-112">**ملاحظه** : إذا قمت بنقل ملكيه الفوترة لاشتراكك إلى حساب مستخدم في مستاجر Azure AD آخر ، ستتم أزاله كافة تعيينات [التحكم بالوصول المستند إلى الدور (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)لأداره الموارد في الاشتراك بشكل دائم.</span><span class="sxs-lookup"><span data-stu-id="1ac3d-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="1ac3d-113">سيتمكن المالك الجديد فقط من الوصول إلى أداره الموارد في الاشتراك.</span><span class="sxs-lookup"><span data-stu-id="1ac3d-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="1ac3d-114">لمزيد من المعلومات ، راجع [نقل الاشتراك إلى مستخدم في مستاجر AZURE AD آخر](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="1ac3d-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="1ac3d-115">**المستندات المستحسنة**</span><span class="sxs-lookup"><span data-stu-id="1ac3d-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="1ac3d-116">نقل ملكيه الفوترة لاشتراك Azure إلى حساب آخر</span><span class="sxs-lookup"><span data-stu-id="1ac3d-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="1ac3d-117">حول تحويل ملكيه الفوترة لاشتراك Azure</span><span class="sxs-lookup"><span data-stu-id="1ac3d-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="1ac3d-118">نقل الرسومات في Visual Studio وشبكه شركاء Microsoft (مبن) والدفع بالاضافه إلى الشركات المطورة/التجريبية</span><span class="sxs-lookup"><span data-stu-id="1ac3d-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="1ac3d-119">نقل الاسئله المتداولة حول الملكية</span><span class="sxs-lookup"><span data-stu-id="1ac3d-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="1ac3d-120">استكشاف مشاكل تحويل الملكية وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="1ac3d-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
