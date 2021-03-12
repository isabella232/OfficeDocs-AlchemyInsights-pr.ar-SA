---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709057"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

هل تعمل مع PowerShell أو البرامج النصية داخل Sharepoint Online؟ تفضل بزيارة الارتباطات الموجودة أدناه للحصول على مزيد من المعلومات.
- [بدء العمل باستخدام SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [الاتصال ب SPO PowerShell باستخدام المصادقة متعددة العوامل (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [يحتوي SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) على مكتبة لأوامر PowerShell التي تسمح لك بتنفيذ إجراءات الإدارة المعقدة تجاه SPO.

> [!NOTE]
> - إذا كنت تواجه مشاكل في الاتصال ب shell إدارة SPO، فتأكد من [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) أنك قمت بتحديث الإصدار الأخير وحاول إعادة استيراد الوحدة النمطية باستخدام *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - إذا كنت تحاول تشغيل البرامج النصية لنموذج العنصر من جانب العميل، ستحتاج إلى تثبيت [SDK](https://www.microsoft.com/download/details.aspx?id=42038) لمكونات عميل Sharepoint Online على جهازك المحلي.
> - إذا كنت تواجه مشاكل في تشغيل البرامج النصية من PowerShell، فقد ترغب في تشغيل PowerShell كمسؤول وتغيير ["نهج التنفيذ".](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)