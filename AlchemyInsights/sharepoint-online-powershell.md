---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830569"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

هل تعمل مع PowerShell أو البرامج النصية ضمن Sharepoint Online؟ تفضل بزيارة الارتباطات أدناه للحصول على مزيد من المعلومات.
- [بدء العمل باستخدام SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [الاتصال ب SPO PowerShell باستخدام المصادقة متعددة العوامل (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [يحتوي SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) على مكتبة من أوامر PowerShell التي تسمح لك بتنفيذ إجراءات الإدارة المعقدة تجاه SPO.

> [!NOTE]
> - إذا كنت تواجه مشاكل في الاتصال ب SPO management shell، فتأكد من [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) أنك قمت بتحديث الإصدار الأخير وحاول إعادة استيراد الوحدة النمطية باستخدام *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - إذا كنت تحاول تشغيل البرامج النصية لنموذج العنصر من جانب العميل، ستحتاج إلى تثبيت [SDK](https://www.microsoft.com/download/details.aspx?id=42038) لمكونات عميل Sharepoint Online على جهازك المحلي.
> - إذا كنت تواجه مشاكل في تشغيل البرامج النصية من PowerShell، فقد تحتاج إلى التفكير في تشغيل PowerShell كمسؤول وتغيير [نهج التنفيذ](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).