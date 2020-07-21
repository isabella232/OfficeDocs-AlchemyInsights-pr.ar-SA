---
title: مستخدم واحد لا يرى الوظائف الإضافية في Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197705"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="c48ee-102">مستخدم واحد لا يرى الوظائف الإضافية في Outlook</span><span class="sxs-lookup"><span data-stu-id="c48ee-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="c48ee-103">قد يكون المستخدم جزءاً من دور لا يحتوي على المعلمة AppsForOfficeEnabled الصحيحة.</span><span class="sxs-lookup"><span data-stu-id="c48ee-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="c48ee-104">تشغيل هذا cmdlet لمعرفة ما إذا كان الدور الصحيح مقترن مع المستخدم:</span><span class="sxs-lookup"><span data-stu-id="c48ee-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="c48ee-105">الحصول على إدارةRoleAssignment -RoleAssignee user@domain.com -تفويض $false | تنسيق-جدول -دور السيارات،RoleAssigneeName،RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="c48ee-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="c48ee-106">لمزيد من المعلومات، راجع [تحديد المسؤولين والمستخدمين الذين يمكنهم تثبيت الوظائف الإضافية لـ Outlook وإدارتها](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="c48ee-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
