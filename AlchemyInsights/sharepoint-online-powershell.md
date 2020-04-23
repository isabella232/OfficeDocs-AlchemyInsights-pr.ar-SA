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
# <a name="sharepoint-online-powershell"></a>Sharepoint على الانترنت باورشيل

العمل مع PowerShell أو البرامج النصية داخل Sharepoint Online؟ قم بزيارة الروابط أدناه للحصول على مزيد من المعلومات.
- [البدء مع SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [الاتصال SPO PowerShell مع مصادقة متعددة العوامل (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [يحتوي أنماط وممارسات SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) على مكتبة من أوامر PowerShell التي تسمح لك بتنفيذ إجراءات إدارة معقدة تجاه SPO.

> [!NOTE]
> - إذا كنت تواجه مشكلات في الاتصال بشل إدارة SPO، فتأكد من تحديثأحدث إصدار ومحاولة [إعادة استيراد الوحدة النمطية](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) باستخدام *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - إذا كنت تحاول تشغيل البرامج النصية طراز كائن من جانب العميل، سوف تحتاج إلى تثبيت [مكونات العميل عبر إنترنت Sharepoint SDK](https://www.microsoft.com/download/details.aspx?id=42038) على الجهاز المحلي الخاص بك.
> - إذا كنت تواجه مشكلات في تشغيل البرامج النصية من PowerShell، فقد تحتاج إلى النظر في تشغيل PowerShell كمسؤول وتغيير [نهج التنفيذ](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).