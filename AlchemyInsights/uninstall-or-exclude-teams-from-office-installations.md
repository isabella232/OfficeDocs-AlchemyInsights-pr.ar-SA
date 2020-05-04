---
title: إلغاء تثبيت الفرق أو استبعادها من عمليات تثبيت Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: b6613733e743e08a9b18b1ada70fde164b0d5dc3
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010277"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>إلغاء تثبيت الفرق أو استبعادها من عمليات تثبيت Office الجديدة أو الموجودة

يتم تضمين Microsoft Teams كجزء من تطبيقات Microsoft 365 للمؤسسات وMicrosoft 365 Apps للأعمال وOffice for Mac.

- استخدم [أداة نشر Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) لاستبعاد الفرق من عمليات التثبيت الجديدة في Office.
- *لإلغاء تثبيت* "الفرق" من جهاز يعمل بنظام التشغيل Windows، راجع إلغاء [تثبيت "فرق Microsoft".](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) لتنظيف Microsoft Teams من أجهزة أو مستخدمين مستهدفين متعددين، راجع [تنظيف نشر Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- استخدم الخيار [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) لمنع Microsoft Teams من التثبيت تلقائيًا باستخدام Office.
- استخدم الخيار [PreventFirstLaunchAfterInstall،](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *قبل تثبيت الفرق*، لمنع Microsoft Teams من البدء تلقائياً بعد التثبيت.

إذا كنت تستخدم Office for Mac، فراجع [عمليات تثبيت Microsoft Teams على Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).