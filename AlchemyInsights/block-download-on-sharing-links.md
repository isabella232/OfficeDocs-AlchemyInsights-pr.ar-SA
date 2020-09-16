---
title: حظر التنزيل علي ارتباطات المشاركة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685729"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="86123-102">حظر التنزيل علي ارتباطات المشاركة</span><span class="sxs-lookup"><span data-stu-id="86123-102">Block download on sharing links</span></span>

<span data-ttu-id="86123-103">يتوفر **تنزيل الكتلة** **للارتباطات لعرض** مستندات Office فقط.</span><span class="sxs-lookup"><span data-stu-id="86123-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="86123-104">عند تحديد هذا الخيار ، لن يتمكن الأشخاص الذين لديهم حق الوصول إلى الملف عبر الارتباط الذي انشاته من رؤية خيارات تنزيل الملف أو طباعته أو نسخه.</span><span class="sxs-lookup"><span data-stu-id="86123-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="86123-105">يمكن للمسؤولين التحكم في ما إذا كان الاعداد "حظر التنزيل" يظهر لملفات Office فقط ام لا عن طريق تغيير `BlockDownloadLinksFileType` الاعداد في [سبوتينانت](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) أو [set سبوسيتي](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="86123-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>
