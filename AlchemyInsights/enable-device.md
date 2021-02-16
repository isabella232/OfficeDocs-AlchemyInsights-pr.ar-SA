---
title: تمكين الجهاز
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256661"
---
# <a name="enable-device"></a>تمكين الجهاز

**لتمكين الجهاز باستخدام أمر Powershell**

قم بتنفيذ الأوامر التالية:

- للحصول على كائن الجهاز: `Get-MsolDevice -Name <Name>`
- لتمكين الجهاز: `Enable-MsolDevice -DeviceId <DeviceId>`

لمزيد من المعلومات حول تكوين الصلة المختلطة على المجالات المدارة، راجع ["تكوين الصلة المختلطة".](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
