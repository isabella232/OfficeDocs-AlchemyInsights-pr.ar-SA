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
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800154"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="ca1d6-102">لا توجد نتائج من محتوى البحث/الصادرات</span><span class="sxs-lookup"><span data-stu-id="ca1d6-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="ca1d6-103">مشاكل مع محتوى البحث/الصادرات عدم إرجاع أية بيانات قد يرجع إلى "تصفية الأمان توافق" معين تم إعداد إدارة معينة وعدم إبلاغه إلى جميع المسؤولين.</span><span class="sxs-lookup"><span data-stu-id="ca1d6-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="ca1d6-104">لحل هذه المشكلة، تحقق من عدم وجود أي "عوامل تصفية أمان التوافق" الذي يمكن أن يسبب هذا:</span><span class="sxs-lookup"><span data-stu-id="ca1d6-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="ca1d6-105">الاتصال بأمان و Powershell مركز التوافق</span><span class="sxs-lookup"><span data-stu-id="ca1d6-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="ca1d6-106">قم بتشغيل كوماندليتس التالية:</span><span class="sxs-lookup"><span data-stu-id="ca1d6-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="ca1d6-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="ca1d6-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="ca1d6-108">الحصول على كومبليانسيسيكوريتيفيلتير-مؤسسة $org</span><span class="sxs-lookup"><span data-stu-id="ca1d6-108">Get-ComplianceSecurityFilter -Organization $org</span></span>