---
title: مستخدم واحد لا يري الوظائف الاضافيه في Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 8c99b443a2d83f3ac24362d63cd6363a66a81393
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719652"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="39f94-102">مستخدم واحد لا يري الوظائف الاضافيه في Outlook</span><span class="sxs-lookup"><span data-stu-id="39f94-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="39f94-103">قد يكون المستخدم جزءا من دور لا يحتوي علي معلمه أبسفوروفيسينابليد الصحيحة.</span><span class="sxs-lookup"><span data-stu-id="39f94-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="39f94-104">قم بتشغيل أمر cmdlet هذا لمعرفه ما إذا كان الدور الصحيح مقترنا بالمستخدم:</span><span class="sxs-lookup"><span data-stu-id="39f94-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="39f94-105">ماناجيمينتروليسيجنمينت-روليسيجني user@domain.com-تفويض $false | تنسيق-الجدول-الدور التلقائي ، روليسيجنينامي ، روليسيجنيتيبي</span><span class="sxs-lookup"><span data-stu-id="39f94-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="39f94-106">للحصول علي مزيد من المعلومات ، راجع [تحديد المسؤولين والمستخدمين الذين يمكنهم تثبيت الوظائف الاضافيه وأدارتها ل Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="39f94-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
