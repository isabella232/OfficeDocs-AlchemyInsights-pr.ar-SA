---
title: نقل المجال بين المستاجرين
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/2/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002570"
- "7305"
ms.openlocfilehash: d696c9d095fb6b2b374d8c5872e94cc7e32dceb8
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/02/2020
ms.locfileid: "49564365"
---
# <a name="transfer-domain-between-tenants"></a><span data-ttu-id="cf8c5-102">نقل المجال بين المستاجرين</span><span class="sxs-lookup"><span data-stu-id="cf8c5-102">Transfer domain between tenants</span></span>

<span data-ttu-id="cf8c5-103">يمكن أزاله مجال مخصص مثل forthcoffee.com يدويا من مستاجر واحد ، ثم التحقق منه في مستاجر جديد.</span><span class="sxs-lookup"><span data-stu-id="cf8c5-103">A custom domain such as forthcoffee.com can be manually removed from one tenant and then verified in a new tenant.</span></span>

<span data-ttu-id="cf8c5-104">اتبع هذه الخطوات [لأزاله مجال](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain).</span><span class="sxs-lookup"><span data-stu-id="cf8c5-104">Follow these steps to [Remove a domain](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/remove-a-domain).</span></span> <span data-ttu-id="cf8c5-105">ثم في المستاجر الجديد ، انتقل إلى **إعدادات**  >  **Domains**  >  **أضافه مجال**.</span><span class="sxs-lookup"><span data-stu-id="cf8c5-105">Then in the new tenant go to **Settings** > **Domains** > **Add domain**.</span></span>

<span data-ttu-id="cf8c5-106">للحصول علي مزيد من السيناريوهات المعقدة ، راجع [العمليات ترحيل الخاصة بالمستاجرين من Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/microsoft-365-tenant-to-tenant-migrations).</span><span class="sxs-lookup"><span data-stu-id="cf8c5-106">For more complex scenarios, see [Microsoft 365 tenant-to-tenant migrations](https://docs.microsoft.com/microsoft-365/enterprise/microsoft-365-tenant-to-tenant-migrations).</span></span>

<span data-ttu-id="cf8c5-107">**ملاحظه أيضا**:</span><span class="sxs-lookup"><span data-stu-id="cf8c5-107">**Also note**:</span></span>
- <span data-ttu-id="cf8c5-108">لا يمكن حذف مجال onmicrosoft.com الاولي أو نقله بين المستاجرين.</span><span class="sxs-lookup"><span data-stu-id="cf8c5-108">The initial onmicrosoft.com domain cannot be deleted or moved between tenants.</span></span>
- <span data-ttu-id="cf8c5-109">لا يمكن نقل مجال مخصص تم شراؤه من Microsoft بين المستاجرين.</span><span class="sxs-lookup"><span data-stu-id="cf8c5-109">A custom domain purchased from Microsoft cannot be moved between tenants.</span></span>