---
title: إلغاء تثبيت Teams أو استبعاده من عمليات تثبيت Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 2d96d54cb479f5f52cc707d4307cf9cf1e891a01
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827779"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>إلغاء تثبيت Teams أو استبعاده من عمليات تثبيت Office الجديدة أو الموجودة

يتم تضمين Microsoft Teams كجزء من تطبيقات Microsoft 365 للمؤسسات وتطبيقات Microsoft 365 للأعمال Macلنظام التشغيل Office.

- استخدم أداة [نشر Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) لاستبعاد Teams من عمليات التثبيت الجديدة ل Office.
- *إلغاء تثبيت* Teams من جهاز يعمل بنظام التشغيل Windows، راجع إلغاء تثبيت Microsoft [Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). لتنظيف Microsoft Teams من أجهزة أو مستخدمين هدفين متعددين، راجع تنظيف نشر [Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- استخدم [الخيار PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) لمنع Microsoft Teams من التثبيت تلقائيا باستخدام Office.
- استخدم [الخيار PreventFirstLaunchAfterInstall،](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) قبل تثبيت *Teams*، لمنع Microsoft Teams من البدء تلقائيا بعد التثبيت.

إذا كنت تستخدم Macلنظام التشغيل Office، فشاهد عمليات تثبيت [Microsoft Teams على جهاز Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).