---
title: حظر التنزيل على روابط المشاركة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357282"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="ffca6-102">حظر التنزيل على روابط المشاركة</span><span class="sxs-lookup"><span data-stu-id="ffca6-102">Block download on sharing links</span></span>

<span data-ttu-id="ffca6-103">يتوفر **تنزيل الحظر** **للارتباطات للعرض فقط** إلى مستندات Office.</span><span class="sxs-lookup"><span data-stu-id="ffca6-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="ffca6-104">عند تحديد هذا الخيار، لن يرى الأشخاص الذين يمكنهم الوصول إلى الملف عبر الرابط الذي أنشأته خيارات لتنزيل الملف أو طباعته أو نسخه.</span><span class="sxs-lookup"><span data-stu-id="ffca6-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="ffca6-105">يمكن للمسؤولين التحكم في ما إذا كان إعداد "تنزيل الكتلة" يظهر فقط لملفات Office أم لا عن طريق تغيير `BlockDownloadLinksFileType` الإعداد في [cmdlets Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) أو [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ffca6-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>
