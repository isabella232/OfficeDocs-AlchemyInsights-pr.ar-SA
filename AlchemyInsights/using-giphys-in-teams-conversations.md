---
title: استخدام Giphys في محادثات الفرق
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982419"
---
# <a name="using-giphys-in-teams-conversations"></a>استخدام Giphys في محادثات الفرق

يتم تمكين الوصول إلى Giphys في دردشة الفرق بشكل افتراضي. بصفتك المسؤول ، يمكنك التحكم في ما إذا كانت Giphys متوفرة للمستخدمين من خلال [تعيين نهج المراسلة](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) والتاكد من ان **استخدام Giphys في المحادثات** قيد **التشغيل**.

إذا لم تعمل صور Gif كما هو متوقع في محادثات الفرق ، فتحقق من:

يحتاج [نهج المراسلة](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) إلى السماح بالGiphys. للتحقق من الصحة باستخدام أوامر PowerShell cmdlets:

- تاكد من انه يمكنك [أداره الفرق باستخدام PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- قم بتشغيل [الكستيمسميساجينجبوليسي العام](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) الخاص بالأمر PowerShell والتحقق من تعيين **اللووجيفي** إلى **TRUE**.
- إذا تم تعيين **اللووجيفي** إلى **FALSE** ، فقم بتشغيل مجموعه أوامر PowerShell [التالية-ال$True اللووجيفي العامة](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)الخاصة بالكستيمسميساجينجبوليسي.

يجب تمكين [التجربة المتصلة الاختيارية](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) للسماح بالوصول إلى عنوان URL لجيفي.

> [!NOTE]
> إذا كان لديك العديد من النهج الخاصة بالمراسلة التي تم تكوينها للمستاجر المستاجر ، فيمكنك تحديد هويه النهج المعين إلى المستخدم المتاثر باستخدام الأمر PowerShell [كسونلينيوسير الحصول علي الهوية](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | حدد تيمسميساجينجبوليسي.
