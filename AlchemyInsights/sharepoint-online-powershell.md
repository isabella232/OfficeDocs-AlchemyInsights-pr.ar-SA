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
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="4be31-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="4be31-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="4be31-103">هل تعمل مع PowerShell أو البرامج النصية داخل Sharepoint Online؟</span><span class="sxs-lookup"><span data-stu-id="4be31-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="4be31-104">تفضل بزيارة الارتباطات الموجودة أدناه للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="4be31-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="4be31-105">بدء العمل باستخدام SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="4be31-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="4be31-106">الاتصال ب SPO PowerShell باستخدام المصادقة متعددة العوامل (MFA)</span><span class="sxs-lookup"><span data-stu-id="4be31-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="4be31-107">[يحتوي SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) على مكتبة لأوامر PowerShell التي تسمح لك بتنفيذ إجراءات الإدارة المعقدة تجاه SPO.</span><span class="sxs-lookup"><span data-stu-id="4be31-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="4be31-108">إذا كنت تواجه مشاكل في الاتصال ب shell إدارة SPO، فتأكد من [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) أنك قمت بتحديث الإصدار الأخير وحاول إعادة استيراد الوحدة النمطية باستخدام *"Import-Module Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="4be31-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="4be31-109">إذا كنت تحاول تشغيل البرامج النصية لنموذج العنصر من جانب العميل، ستحتاج إلى تثبيت [SDK](https://www.microsoft.com/download/details.aspx?id=42038) لمكونات عميل Sharepoint Online على جهازك المحلي.</span><span class="sxs-lookup"><span data-stu-id="4be31-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="4be31-110">إذا كنت تواجه مشاكل في تشغيل البرامج النصية من PowerShell، فقد ترغب في تشغيل PowerShell كمسؤول وتغيير ["نهج التنفيذ".](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="4be31-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>