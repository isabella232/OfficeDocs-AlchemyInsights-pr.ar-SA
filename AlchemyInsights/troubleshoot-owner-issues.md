---
title: استكشاف مشاكل المالك وإصلاحها
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900729"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="2faeb-102">استكشاف مشاكل المالك وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="2faeb-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="2faeb-103">لاستكشاف المشاكل المتعلقة بالمالك وإصلاحها ، نفذ الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="2faeb-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="2faeb-104">[أضافه مسؤولي الاشتراك في azure أو تغييرهم](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): مجموعات Azure active Directory (azure AD) مملوكه ومداره من قبل مالكي المجموعة.</span><span class="sxs-lookup"><span data-stu-id="2faeb-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="2faeb-105">يمكن لمالكي المجموعة المستخدمين أو أساسيات الخدمة ، ويمكنهم أداره المجموعة ، بما في ذلك العضوية.</span><span class="sxs-lookup"><span data-stu-id="2faeb-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="2faeb-106">مالكو المجموعة أو المجموعات الحالية فقط يمكنهم تعيين مالكي المجموعة.</span><span class="sxs-lookup"><span data-stu-id="2faeb-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="2faeb-107">لا يجب ان يكون مالكو المجموعة أعضاء في المجموعة.</span><span class="sxs-lookup"><span data-stu-id="2faeb-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="2faeb-108">[أضافه مسؤولي الاشتراك في Azure أو تغييرهم](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): تصف هذه المقالة كيفيه أضافه دور المسؤول أو تغييره لمستخدم يستخدم Azure RBAC في نطاق الاشتراك.</span><span class="sxs-lookup"><span data-stu-id="2faeb-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="2faeb-109">استخدم PowerShell لأضافه مالك مجموعه أو مالك تطبيق.</span><span class="sxs-lookup"><span data-stu-id="2faeb-109">Use PowerShell to add a group owner or an application owner.</span></span>
