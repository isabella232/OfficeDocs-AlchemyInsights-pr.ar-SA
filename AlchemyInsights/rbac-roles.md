---
title: 'ادوار RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583172"
---
# <a name="rbac-rules"></a><span data-ttu-id="24088-102">قواعد RBAC</span><span class="sxs-lookup"><span data-stu-id="24088-102">RBAC rules</span></span>

<span data-ttu-id="24088-103">إذا حصلت علي خطا في الاذن:</span><span class="sxs-lookup"><span data-stu-id="24088-103">If you get the permission error:</span></span> 

- <span data-ttu-id="24088-104">لا **يتضمن العميل الذي يحتوي علي معرف العنصر تخويلا لتنفيذ الاجراء فوق النطاق (التعليمات البرمجية: أوثوريزاتيونفايليد)**: عند محاولة إنشاء مورد ، تاكد من انك قمت بتسجيل الدخول حاليا باستخدام مستخدم تم تعيين دور له اذن كتابه إلى المورد في النطاق المحدد.</span><span class="sxs-lookup"><span data-stu-id="24088-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="24088-105">علي سبيل المثال ، لأداره الاجهزه الظاهرية في مجموعه موارد ، يجب ان يتوفر لديك دور [المساهم في الجهاز الظاهري](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) علي مجموعه الموارد (أو النطاق الأصلي).</span><span class="sxs-lookup"><span data-stu-id="24088-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="24088-106">للحصول علي قائمه بالأذونات لكل دور مضمن ، راجع [الأدوار المضمنة لموارد Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="24088-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="24088-107">**ليس لديك الاذن لإنشاء طلب دعم**: عند محاولة إنشاء بطاقة دعم أو تحديثها ، تاكد من انك قمت بتسجيل الدخول حاليا باستخدام المستخدم الذي تم تعيين دور له الذي يملك الاذن Microsoft. الدعم/سوبورتيكيتس/الكتابة ، مثل [الدعم المعتمد للطلب](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="24088-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="24088-108">**لا يمكن إنشاء المزيد من تعيينات الأدوار (التعليمات البرمجية: روليسيجنمينتليميتيكسسيديد)**: عند محاولة تعيين دور ، حاول تقليل عدد تعيينات الدور عن طريق تعيين ادوار إلى المجموعات بدلا من ذلك.</span><span class="sxs-lookup"><span data-stu-id="24088-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="24088-109">يدعم Azure تعيينات الأدوار حتى **2000** لكل اشتراك.</span><span class="sxs-lookup"><span data-stu-id="24088-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="24088-110">للحصول علي مزيد من التفاصيل حول ادوار Azure RBAC ، راجع [ادوار AZURE RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="24088-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
