---
title: لم يتم إرجاع اي نتائج اثناء البحث في المحتوي/التصدير
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727210"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="3aa52-102">لم يتم إرجاع اي نتائج اثناء البحث في المحتوي/التصدير</span><span class="sxs-lookup"><span data-stu-id="3aa52-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="3aa52-103">إذا كنت تواجه مشاكل في سيناريوهات eDiscovery التالية:</span><span class="sxs-lookup"><span data-stu-id="3aa52-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="3aa52-104">لا ترجع ميزه البحث في المحتوي/التصدير اي بيانات أو بيانات غير متوقعه</span><span class="sxs-lookup"><span data-stu-id="3aa52-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="3aa52-105">فشل البحث عن eDiscovery أو تصديره</span><span class="sxs-lookup"><span data-stu-id="3aa52-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="3aa52-106">قد يرجع ذلك إلى عوامل تصفيه أمان توافق معينه تم اعدادها بواسطة مسؤول معين ولم يتم الإبلاغ عن كل المسؤولين.</span><span class="sxs-lookup"><span data-stu-id="3aa52-106">This may be due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="3aa52-107">لحل هذه المشكلة ، تحقق مما إذا كانت هناك اي عوامل تصفيه أمان للتوافق قد تؤدي إلى حدوث هذه المشاكل:</span><span class="sxs-lookup"><span data-stu-id="3aa52-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="3aa52-108">الاتصال بمركز التوافق والأمان Powershell</span><span class="sxs-lookup"><span data-stu-id="3aa52-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="3aa52-109">قم بتشغيل الكوماندليتس التالية:</span><span class="sxs-lookup"><span data-stu-id="3aa52-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="3aa52-110">للحصول علي معلومات اضافيه حول عوامل تصفيه أمان التوافق ، راجع [تصفيه الأذونات للبحث في المحتوي](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="3aa52-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
