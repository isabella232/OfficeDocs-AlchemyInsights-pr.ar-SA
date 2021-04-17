---
title: لا تتم مزامنة Active Directory
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822838"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="05a4c-102">لا تتم مزامنة Active Directory</span><span class="sxs-lookup"><span data-stu-id="05a4c-102">Active Directory not syncing</span></span>

<span data-ttu-id="05a4c-103">إذا كنت تتلقى أخطاء في المزامنة، مثل "لا توجد مزامنة حديثة"، أو لاحظت حالة مزامنة الدليل في مدخل مسؤول Office، تقول "آخر مزامنة منذ أكثر من 3 أيام"، فقد يكون لدى AADConnect إعدادات غير صحيحة أو أذونات غير كافية لتنفيذ المزامنة.</span><span class="sxs-lookup"><span data-stu-id="05a4c-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="05a4c-104">قد يؤدي إعادة تثبيت AADConnect باستخدام الإعدادات المعبرة إلى حل المشكلة بسرعة:</span><span class="sxs-lookup"><span data-stu-id="05a4c-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="05a4c-105">[قم بتنزيل أحدث إصدار من AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="05a4c-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="05a4c-106">[اتبع إرشادات التثبيت السريع.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="05a4c-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="05a4c-107">لمزيد من المعلومات حول حسابات خدمة AADConnect، راجع [Azure AD Connect: الحسابات والأذونات](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="05a4c-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
