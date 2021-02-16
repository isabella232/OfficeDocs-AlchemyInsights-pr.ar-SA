---
title: مزامنة المجموعة
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256652"
---
# <a name="group-sync"></a><span data-ttu-id="b0cc9-102">مزامنة المجموعة</span><span class="sxs-lookup"><span data-stu-id="b0cc9-102">Group sync</span></span>

<span data-ttu-id="b0cc9-103">توفر هذه المقالة إرشادات حول مزامنة المجموعة.</span><span class="sxs-lookup"><span data-stu-id="b0cc9-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="b0cc9-104">إذا لم يتمكن المسؤول العام أو مالك المجموعة من تعديل خصائص المجموعة أو إضافة أعضاء أو تعيين مالكين في مدخل Azure، فتأكد من أن مصدر مرجع المجموعة هو Azure Active Directory (Azure AD) للمسؤول العام أو مالك المجموعة لتعديل المجموعة.</span><span class="sxs-lookup"><span data-stu-id="b0cc9-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="b0cc9-105">قبل محاولة حذف مجموعة متزامنة في Azure AD، تأكد من حذف جميع التراخيص المعينة لتجنب الأخطاء. [](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced)</span><span class="sxs-lookup"><span data-stu-id="b0cc9-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="b0cc9-106">لمعرفة كيفية مزامنة المستخدمين والمجموعات وجهات الاتصال، راجع [مزامنة Azure AD Connect،](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)واتبع مزامنة مجموعة في موقع Azure باستخدام [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) لمزامنة المجموعات المحلية باستخدام AD connect.</span><span class="sxs-lookup"><span data-stu-id="b0cc9-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="b0cc9-107">اتبع هذا الدليل حول استكشاف الأخطاء [وإصلاحها](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) أثناء المزامنة استكشاف الأخطاء الشائعة أثناء المزامنة وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="b0cc9-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

