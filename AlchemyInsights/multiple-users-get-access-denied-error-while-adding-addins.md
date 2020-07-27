---
title: يحصل العديد من المستخدمين على خطأ تم رفض الوصول أثناء إضافة الوظائف الإضافية في Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423304"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="6acff-102">يحصل العديد من المستخدمين على خطأ تم رفض الوصول أثناء إضافة الوظائف الإضافية في Outlook</span><span class="sxs-lookup"><span data-stu-id="6acff-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="6acff-103">يمكنك تحديد المسؤولين في المؤسسة التي لديك أذونات لتثبيت الوظائف الإضافية لـ Outlook وإدارتها.</span><span class="sxs-lookup"><span data-stu-id="6acff-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="6acff-104">يمكنك أيضاً تحديد المستخدمين الذين لديهم إذن في مؤسستك لتثبيت الوظائف الإضافية وإدارتها لاستخدامهم الخاص.</span><span class="sxs-lookup"><span data-stu-id="6acff-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="6acff-105">للحصول على التفاصيل، راجع [تحديد المسؤولين والمستخدمين الذين يمكنهم تثبيت الوظائف الإضافية لـ Outlook وإدارتها](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="6acff-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="6acff-106">للتحقق من أنك قمت بتعيين الأذونات لمستخدم بنجاح، استبدل <Role Name> باسم الدور للتحقق من صحة، ثم قم بتشغيل الأمر التالي في Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="6acff-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="6acff-107">الحصول على إدارةRoleAssignment -دور " <Role Name> - GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="6acff-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="6acff-108">يوضح لك هذا المثال كيفية التحقق من الأشخاص الذين قمت بتعيينهم للأذونات لتثبيت الوظائف الإضافية من متجر Office للمؤسسة.</span><span class="sxs-lookup"><span data-stu-id="6acff-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="6acff-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="6acff-109">PowerShell</span></span>

<span data-ttu-id="6acff-110">-Role "Org Marketplace Apps" - GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="6acff-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="6acff-111">في النتائج، Get-ManagementRoleAssignment، راجع الإدخالات في العمود "المستخدمين الفعالين".</span><span class="sxs-lookup"><span data-stu-id="6acff-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="6acff-112">للحصول على معلومات تفصيلية عن بناء الجملة والمعلمة، راجع [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="6acff-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 