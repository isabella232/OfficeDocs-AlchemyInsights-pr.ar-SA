---
title: Sharepoint باور شيل على الانترنت
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/23/2019
ms.locfileid: "37122986"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="d098d-102">Sharepoint باور شيل على الانترنت</span><span class="sxs-lookup"><span data-stu-id="d098d-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="d098d-103">العمل مع PowerShell أو البرامج النصية داخل Sharepoint عبر الإنترنت؟</span><span class="sxs-lookup"><span data-stu-id="d098d-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="d098d-104">قم بزيارة الروابط أدناه للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="d098d-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="d098d-105">الشروع في العمل مع SharePoint إدارة على الانترنت شل</span><span class="sxs-lookup"><span data-stu-id="d098d-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="d098d-106">الاتصال بـ SPO PowerShell مع المصادقة متعددة العوامل (MFA)</span><span class="sxs-lookup"><span data-stu-id="d098d-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="d098d-107">يحتوي [SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) على مكتبة من أوامر PowerShell تسمح لك بتنفيذ إجراءات إدارة معقدة تجاه SPO.</span><span class="sxs-lookup"><span data-stu-id="d098d-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="d098d-108">إذا كنت تواجه مشكلات في الاتصال بshell إدارة SPO تأكد من تحديث إلى أحدث إصدار ثم حاول [إعادة استيراد الوحدة النمطية](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) باستخدام *"استيراد الوحدة النمطية Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="d098d-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="d098d-109">إذا كنت تحاول تشغيل البرامج النصية طراز كائن العميل، ستحتاج إلى تثبيت [SDK مكونات عميل Sharepoint عبر إنترنت](https://www.microsoft.com/download/details.aspx?id=42038) على الجهاز المحلي.</span><span class="sxs-lookup"><span data-stu-id="d098d-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="d098d-110">إذا كنت تواجه مشكلات في تشغيل البرامج النصية من PowerShell، فقد تحتاج إلى تشغيل PowerShell كمسؤول وتغيير [نهج التنفيذ](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="d098d-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>