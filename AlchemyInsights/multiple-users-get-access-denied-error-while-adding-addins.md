---
title: ظهور رسالة الخطا "رفض الوصول" لعده مستخدمين اثناء أضافه وظائف اضافيه في Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724350"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="78b89-102">ظهور رسالة الخطا "رفض الوصول" لعده مستخدمين اثناء أضافه وظائف اضافيه في Outlook</span><span class="sxs-lookup"><span data-stu-id="78b89-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="78b89-103">يمكنك تحديد المسؤولين الذين لديهم الأذونات لتثبيت الوظائف الاضافيه وأدارتها ل Outlook.</span><span class="sxs-lookup"><span data-stu-id="78b89-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="78b89-104">يمكنك أيضا تحديد المستخدمين الذين لديهم الاذن لتثبيت الوظائف الاضافيه وأدارتها لاستخدامها.</span><span class="sxs-lookup"><span data-stu-id="78b89-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="78b89-105">للحصول علي التفاصيل ، راجع [تحديد المسؤولين والمستخدمين الذين يمكنهم تثبيت الوظائف الاضافيه وأدارتها ل Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="78b89-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="78b89-106">للتحقق من انك قمت بتعيين الأذونات لمستخدم بنجاح ، استبدل <Role Name> باسم الدور الذي تريد التحقق منه ، ثم قم بتشغيل الأمر التالي في Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="78b89-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="78b89-107">ماناجيمينتروليسيجنمينت-Role " <Role Name> "-جيتيفيكتيفيوسيرس</span><span class="sxs-lookup"><span data-stu-id="78b89-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="78b89-108">يوضح هذا المثال كيفيه التحقق من الأشخاص الذين قمت بتعيين أذونات لهم لتثبيت الوظائف الاضافيه من متجر Office للمؤسسة.</span><span class="sxs-lookup"><span data-stu-id="78b89-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="78b89-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="78b89-109">PowerShell</span></span>

<span data-ttu-id="78b89-110">-الدور "التطبيقات الخاصة بسوق المؤسسة"-جيتيفيكتيفيوسيرس</span><span class="sxs-lookup"><span data-stu-id="78b89-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="78b89-111">في النتائج ، ماناجيمينتروليسيجنمينت ، راجع الإدخالات في العمود المستخدمون الفعالون.</span><span class="sxs-lookup"><span data-stu-id="78b89-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="78b89-112">للحصول علي معلومات تفصيليه حول المعلمات وبناءها ، راجع [ماناجيمينتروليسيجنمينت](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="78b89-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 