---
title: لا يوجد نتائج البحث المحتوى
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516766"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="00774-102">لا توجد نتائج من محتوى البحث/الصادرات</span><span class="sxs-lookup"><span data-stu-id="00774-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="00774-103">مشاكل مع محتوى البحث/الصادرات عدم إرجاع أية بيانات قد يرجع إلى "تصفية الأمان توافق" معين تم إعداد إدارة معينة وعدم إبلاغه إلى جميع المسؤولين.</span><span class="sxs-lookup"><span data-stu-id="00774-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="00774-104">لحل هذه المشكلة، تحقق من عدم وجود أي "عوامل تصفية أمان التوافق" الذي يمكن أن يسبب هذا:</span><span class="sxs-lookup"><span data-stu-id="00774-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="00774-105">الاتصال بأمان و Powershell مركز التوافق</span><span class="sxs-lookup"><span data-stu-id="00774-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="00774-106">قم بتشغيل كوماندليتس التالية:</span><span class="sxs-lookup"><span data-stu-id="00774-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="00774-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="00774-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="00774-108">الحصول على كومبليانسيسيكوريتيفيلتير-مؤسسة $org</span><span class="sxs-lookup"><span data-stu-id="00774-108">Get-ComplianceSecurityFilter -Organization $org</span></span>