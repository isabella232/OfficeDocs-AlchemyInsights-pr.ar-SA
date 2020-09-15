---
title: إلغاء تثبيت الفرق أو استبعادها من عمليات تثبيت Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658208"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="42d08-102">إلغاء تثبيت الفرق أو استبعادها من تثبيتات Office الجديدة أو الموجودة</span><span class="sxs-lookup"><span data-stu-id="42d08-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="42d08-103">يتم تضمين فرق microsoft كجزء من تطبيقات Microsoft 365 ل enterprise و Microsoft 365 Apps for business و Office for Mac.</span><span class="sxs-lookup"><span data-stu-id="42d08-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="42d08-104">استخدم [أداه النشر من office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) لاستبعاد الفرق من التثبيتات الجديدة ل office.</span><span class="sxs-lookup"><span data-stu-id="42d08-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="42d08-105">*للغاء تثبيت* الفرق من جهاز يقوم بتشغيل Windows ، راجع [أزاله تثبيت فرق Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="42d08-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="42d08-106">لتنظيف فرق Microsoft من الاجهزه المستهدفة أو المستخدمين المتعددين ، راجع [التنظيف النظيف لنشر فرق microsoft](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="42d08-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="42d08-107">استخدم خيار [بريفينتيمسينستال](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) لمنع التثبيت التلقائي لفرق Microsoft باستخدام Office.</span><span class="sxs-lookup"><span data-stu-id="42d08-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="42d08-108">استخدم الخيار [بريفينتفيرستلاونتشافتيرينستال](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) ، *قبل تثبيت الفرق*، لمنع فرق Microsoft من بدء التشغيل تلقائيا بعد التثبيت.</span><span class="sxs-lookup"><span data-stu-id="42d08-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="42d08-109">إذا كنت تستخدم Office for Mac ، فراجع [تثبيتات فرق Microsoft علي جهاز Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="42d08-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>