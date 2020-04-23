---
title: Sharepoint على الانترنت باورشيل
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764248"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="1733c-102">Sharepoint على الانترنت باورشيل</span><span class="sxs-lookup"><span data-stu-id="1733c-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="1733c-103">العمل مع PowerShell أو البرامج النصية داخل Sharepoint Online؟</span><span class="sxs-lookup"><span data-stu-id="1733c-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="1733c-104">قم بزيارة الروابط أدناه للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="1733c-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="1733c-105">البدء مع SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="1733c-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="1733c-106">الاتصال SPO PowerShell مع مصادقة متعددة العوامل (MFA)</span><span class="sxs-lookup"><span data-stu-id="1733c-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="1733c-107">[يحتوي أنماط وممارسات SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) على مكتبة من أوامر PowerShell التي تسمح لك بتنفيذ إجراءات إدارة معقدة تجاه SPO.</span><span class="sxs-lookup"><span data-stu-id="1733c-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="1733c-108">إذا كنت تواجه مشكلات في الاتصال بشل إدارة SPO، فتأكد من تحديثأحدث إصدار ومحاولة [إعادة استيراد الوحدة النمطية](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) باستخدام *"Import-Module Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="1733c-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="1733c-109">إذا كنت تحاول تشغيل البرامج النصية طراز كائن من جانب العميل، سوف تحتاج إلى تثبيت [مكونات العميل عبر إنترنت Sharepoint SDK](https://www.microsoft.com/download/details.aspx?id=42038) على الجهاز المحلي الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="1733c-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="1733c-110">إذا كنت تواجه مشكلات في تشغيل البرامج النصية من PowerShell، فقد تحتاج إلى النظر في تشغيل PowerShell كمسؤول وتغيير [نهج التنفيذ](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="1733c-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>