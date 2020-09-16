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
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770826"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="2c590-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="2c590-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="2c590-103">هل تستخدم PowerShell أو البرامج النصية ضمن Sharepoint Online ؟</span><span class="sxs-lookup"><span data-stu-id="2c590-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="2c590-104">قم بزيارة الارتباطات أدناه للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="2c590-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="2c590-105">بدء استخدام SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="2c590-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="2c590-106">الاتصال ب SPO PowerShell باستخدام مصادقه متعدد (MFA)</span><span class="sxs-lookup"><span data-stu-id="2c590-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="2c590-107">تحتوي [أنماط SharePoint والممارسات (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) علي مكتبه لأوامر PowerShell التي تسمح لك بتنفيذ إجراءات الاداره المعقدة باتجاه SPO.</span><span class="sxs-lookup"><span data-stu-id="2c590-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="2c590-108">إذا كنت تواجه مشاكل في الاتصال باستخدام SPO management shell ، فتاكد من انك قمت بتحديث الإصدار الأخير وحاول [أعاده استيراد الوحدة النمطية](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) باستخدام *"الاستيراد-الوحدة النمطية Microsoft.*</span><span class="sxs-lookup"><span data-stu-id="2c590-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="2c590-109">إذا كنت تحاول تشغيل البرامج النصية لنموذج الكائن من جانب العميل ، ستحتاج إلى تثبيت [SDK مكونات عميل Sharepoint Online](https://www.microsoft.com/download/details.aspx?id=42038) علي جهازك المحلي.</span><span class="sxs-lookup"><span data-stu-id="2c590-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="2c590-110">إذا كنت تواجه مشاكل في تشغيل البرامج النصية من PowerShell ، فقد تحتاج إلى تشغيل PowerShell كمسؤول وتغيير [نهج التنفيذ](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="2c590-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>