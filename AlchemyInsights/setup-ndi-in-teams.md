---
title: تشغيل تقنية NDI
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
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935068"
---
# <a name="turn-on-ndi-technology"></a>تشغيل تقنية NDI

تتطلب تقنية NDI تشغيل خطوتين للمستخدم:

1. يجب على مسؤول المستأجر تمكين الخاصية 'AllowNDIStreaming' في CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. بعد نشر هذا التغيير، يجب على المستخدم تشغيل تقنية NDI® للعميل المحدد من **الإعدادات > الأذونات.**

لمزيد من المعلومات، راجع [استخدام تقنية NDI في Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
