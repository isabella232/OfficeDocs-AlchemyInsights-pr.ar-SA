---
title: لا توجد نتائج في البحث عن المحتوي
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680634"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="8aea2-102">لا توجد نتائج من البحث في المحتوي/التصديرات</span><span class="sxs-lookup"><span data-stu-id="8aea2-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="8aea2-103">المشاكل المتعلقة بالبحث في المحتوي/عمليات التصدير لا يتم إرجاع اي بيانات بسبب عامل تصفيه أمان توافق معين تم اعداده من قبل مسؤول معين ولا يتم الاتصال به لجميع المسؤولين.</span><span class="sxs-lookup"><span data-stu-id="8aea2-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="8aea2-104">لحل هذه المشكلة ، تحقق لمعرفه ما إذا كانت هناك اي عوامل تصفيه أمان للتوافق قد تؤدي إلى ذلك:</span><span class="sxs-lookup"><span data-stu-id="8aea2-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="8aea2-105">الاتصال بمركز التوافق والأمان Powershell</span><span class="sxs-lookup"><span data-stu-id="8aea2-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="8aea2-106">قم بتشغيل الكوماندليتس التالية:</span><span class="sxs-lookup"><span data-stu-id="8aea2-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="8aea2-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="8aea2-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="8aea2-108">كومبليانسيسيكوريتيفيلتير-مؤسسه $org</span><span class="sxs-lookup"><span data-stu-id="8aea2-108">Get-ComplianceSecurityFilter -Organization $org</span></span>