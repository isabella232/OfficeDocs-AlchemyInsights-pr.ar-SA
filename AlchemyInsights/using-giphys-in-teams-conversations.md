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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104295"
---
# <a name="using-giphys-in-teams-conversations"></a>استخدام Giphys في Teams المحادثات

يتم تمكين الوصول إلى giphys Teams المحادثة بشكل افتراضي. كمسؤول، يمكنك التحكم في ما إذا كانت [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) Giphys متوفرة للمستخدمين من خلال تعيين نهج مراسلة والتأكد من أن **استخدام Giphys** في المحادثات هو **على .**

إذا لم تعمل "فوف" كما هو متوقع في Teams المحادثات، فتحقق مما يلي:

يجب [أن يسمح نهج المراسلة](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) ب Giphys. للتحقق باستخدام PowerShell cmdlets:

- تحقق من أنه يمكنك إدارة [Teams باستخدام PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- قم بتشغيل الأمر PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) وتحقق من تعيين **AllowGiphy** إلى **TRUE**.
- إذا **تم تعيين AllowGiphy** إلى **FALSE**، ف قم بتشغيل الأمر PowerShell [التالي Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[يجب تمكين التجارب الاختيارية](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) المتصلة للسماح بالوصول إلى عنوان URL الخاص ب Giphy.

> [!NOTE]
> إذا تم تكوين Teams متعددة للمستأجر، يمكنك تحديد هوية النهج المعين للمستخدم المتأثير باستخدام الأمر [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | حدد TeamsMessagingPolicy.
