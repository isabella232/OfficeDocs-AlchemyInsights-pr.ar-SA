---
title: استخدام Giphys في Teams المحادثات
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
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323507"
---
# <a name="using-giphys-in-teams-conversations"></a>استخدام Giphys في Teams المحادثات

يتم تمكين الوصول إلى giphys Teams المحادثة بشكل افتراضي. كمسؤول، يمكنك التحكم في ما إذا كانت [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) Giphys متوفرة للمستخدمين من خلال تعيين نهج مراسلة والتأكد من أن **استخدام Giphys** في المحادثات هو **على .**

إذا لم تعمل "فوف" كما هو متوقع في Teams المحادثات، فتحقق مما يلي:

يجب [أن يسمح نهج المراسلة](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) ب Giphys. للتحقق باستخدام PowerShell cmdlets:

- تحقق من أنه يمكنك [إدارة Teams باستخدام PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- قم بتشغيل الأمر PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) وتحقق من تعيين **AllowGiphy** إلى **TRUE**.
- إذا **تم تعيين AllowGiphy** إلى **FALSE**، ف قم بتشغيل الأمر PowerShell [التالي Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[يجب تمكين التجارب الاختيارية](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) المتصلة للسماح بالوصول إلى عنوان URL الخاص ب Giphy.

**ملاحظة:** إذا تم تكوين نهج مراسلة Teams متعددة للمستأجر، يمكنك تحديد هوية النهج المعين للمستخدم المتأثير باستخدام الأمر [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | حدد TeamsMessagingPolicy.
