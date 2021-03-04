---
title: التدقيق في Microsoft 365
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429253"
---
# <a name="auditing-in-microsoft-365"></a><span data-ttu-id="9218d-102">التدقيق في Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9218d-102">Auditing in Microsoft 365</span></span>

<span data-ttu-id="9218d-103">إليك بعض الأمور التي يجب معرفتها حول التدقيق في Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="9218d-103">Here are a few things you should know about auditing in Microsoft 365:</span></span>

1. <span data-ttu-id="9218d-104">يتم تدقيق أنشطة مسؤول Exchange بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="9218d-104">Exchange admin activities are audited by default.</span></span>
1. <span data-ttu-id="9218d-105">نحن في عملية تشغيل تدقيق علبة البريد بشكل افتراضي لجميع المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="9218d-105">We're in the process of turning on mailbox auditing by default for all users.</span></span> <span data-ttu-id="9218d-106">لقراءة المزيد حول هذا الأمر، انقر [هنا.](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171)</span><span class="sxs-lookup"><span data-stu-id="9218d-106">To read more about this, click [here](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span></span> <span data-ttu-id="9218d-107">حتى ذلك الحين، إذا كنت تريد الحصول على إرشادات لتمكينها يدويا لشخص واحد أو مؤسسة بأكملها، فاختر الزر "تشغيل تدقيق علبة البريد" أدناه.</span><span class="sxs-lookup"><span data-stu-id="9218d-107">Until then, if you want instructions to manually enable it for one person or an entire organization, choose the Turn on mailbox auditing button below.</span></span>
1. <span data-ttu-id="9218d-108">لا تدعم علب بريد مجموعات Microsoft 365 علب بريد المجلد العام تسجيل التدقيق.</span><span class="sxs-lookup"><span data-stu-id="9218d-108">Microsoft 365 Groups mailboxes and Public Folder mailboxes do not support audit logging.</span></span>
1. <span data-ttu-id="9218d-109">بالنسبة إلى SharePoint/OneDrive، لا يوجد تكوين إضافي مطلوب لتمكين التدقيق.</span><span class="sxs-lookup"><span data-stu-id="9218d-109">For SharePoint/OneDrive, there is no additional configuration required to enabled auditing.</span></span> <span data-ttu-id="9218d-110">لمعرفة الأنشطة التي يتم تدقيقها، راجع:</span><span class="sxs-lookup"><span data-stu-id="9218d-110">To learn what activities are audited, see:</span></span>
    1. [<span data-ttu-id="9218d-111">أنشطة الملفات</span><span class="sxs-lookup"><span data-stu-id="9218d-111">File activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [<span data-ttu-id="9218d-112">أنشطة المجلد</span><span class="sxs-lookup"><span data-stu-id="9218d-112">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. <span data-ttu-id="9218d-113">[أنشطة المشاركة والوصول.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)</span><span class="sxs-lookup"><span data-stu-id="9218d-113">[Sharing and Access activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span></span>
1. <span data-ttu-id="9218d-114">للحصول على قائمة بكل الأنشطة التي تم تدقيقها حسب الخدمة، راجع [الأنشطة التي تم تدقيقها.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)</span><span class="sxs-lookup"><span data-stu-id="9218d-114">For a list of all audited activities by service, see [Audited activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>
