---
title: الدليل النشط لا تتم مزامنته
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265113"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="e7c9f-102">الدليل النشط لا تتم مزامنته</span><span class="sxs-lookup"><span data-stu-id="e7c9f-102">Active Directory not syncing</span></span>

<span data-ttu-id="e7c9f-103">إذا كنت تتلقى أخطاء المزامنة، مثل "لا مزامنة حديثة"، أو لاحظ حالة مزامنة الدليل في بوابة مسؤول Office يقول: "آخر مزامنة منذ أكثر من 3 أيام"، قد يكون AADConnect لديه إعدادات غير صحيحة أو غير كافية أذونات لتنفيذ مزامنة.</span><span class="sxs-lookup"><span data-stu-id="e7c9f-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="e7c9f-104">إعادة تثبيت AADConnect باستخدام إعدادات صريحة قد حل المشكلة بسرعة:</span><span class="sxs-lookup"><span data-stu-id="e7c9f-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="e7c9f-105">[تحميل أحدث إصدار من AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="e7c9f-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="e7c9f-106">[اتبع التعليمات الخاصة بالتثبيت السريع.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="e7c9f-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="e7c9f-107">لمزيد من المعلومات حول حسابات خدمة AADConnect، راجع [Azure AD Connect: الحسابات والأذونات](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="e7c9f-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
