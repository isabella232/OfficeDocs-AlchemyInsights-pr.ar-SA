---
title: مشاكل مالك تسجيل التطبيق
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404151"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="b60f2-102">مشاكل مالك تسجيل التطبيق</span><span class="sxs-lookup"><span data-stu-id="b60f2-102">App Registration Owner issues</span></span>

<span data-ttu-id="b60f2-103">فيما يلي الأساليب المتوفرة لإضافة الأساسيات كملاك لتسجيلات التطبيقات:</span><span class="sxs-lookup"><span data-stu-id="b60f2-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="b60f2-104">استخدام وحدة Azure AD PowerShell النمطية -</span><span class="sxs-lookup"><span data-stu-id="b60f2-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="b60f2-105">المرجع: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="b60f2-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="b60f2-106">استخدام Azure CLI - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="b60f2-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="b60f2-107">المرجع: [مالك تطبيق az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="b60f2-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="b60f2-108">استخدام MS Graph -</span><span class="sxs-lookup"><span data-stu-id="b60f2-108">Using MS Graph -</span></span>

    <span data-ttu-id="b60f2-109">المرجع: [إضافة مالك - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="b60f2-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="b60f2-110">استخدام مدخل Azure AD - انتقل إلى portal.azure.com [>](https://portal.azure.com/) Azure Active directory > تسجيل التطبيقات > حدد تطبيقك > مالكو > إضافة مالكين</span><span class="sxs-lookup"><span data-stu-id="b60f2-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="b60f2-111">**هل يتعذر عليك عرض التطبيق على شفرة تسجيلات التطبيق على الرغم من أنك مالك هذا التطبيق؟**</span><span class="sxs-lookup"><span data-stu-id="b60f2-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="b60f2-112">لا يكون مالك التطبيق دورا إداريا.</span><span class="sxs-lookup"><span data-stu-id="b60f2-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="b60f2-113">إذا تم تمكين الإعداد تقييد الوصول إلى مدخل إدارة [Azure AD،](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) سيكون المسؤول فقط قادرا على عرض التطبيقات على مدخل تسجيل التطبيق.</span><span class="sxs-lookup"><span data-stu-id="b60f2-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="b60f2-114">لكي يتمكن المالك من عرض التطبيقات، قم إما بتعطيل هذا الإعداد (تعيين هذا الإعداد إلى لا) أو تعيين دور المسؤول إلى المالك للتطبيق المحدد فقط.</span><span class="sxs-lookup"><span data-stu-id="b60f2-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="b60f2-115">على الرغم من ذلك، سوف تحتاج إلى ترخيص Azure AD Premium P2 وتمكين [إدارة الهوية المتميزة.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="b60f2-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
