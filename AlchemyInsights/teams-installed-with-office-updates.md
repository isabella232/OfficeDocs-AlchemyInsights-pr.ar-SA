---
title: Teams مثبتا Office التحديثات
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
- "2599"
- "9000140"
- "9000660"
- "2509"
ms.openlocfilehash: c473a001d1441362baad9feb44323b46f1cef42d3c431ef87f0fb0172f10d152
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048719"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>Microsoft Teams تثبيته Office التحديثات

Microsoft Teams كجزء من عمليات  التثبيت الجديدة Microsoft 365 Apps for enterprise Microsoft 365 Apps for business Office for Mac. لمزيد من المعلومات، راجع [متى Microsoft Teams يتم تضمينه مع عمليات](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps) التثبيت الجديدة Office؟

بالإضافة إلى ذلك، بدءا من الإصدار 1906 في القناة الحالية،  سيضاف Teams تدريجيا إلى عمليات التثبيت الموجودة ل Microsoft 365 Apps for enterprise (و Microsoft 365 Apps for business) على الأجهزة التي تعمل ب Windows عند تحديث التثبيت الحالي إلى الإصدار الأخير. لمزيد من المعلومات، راجع ماذا عن عمليات التثبيت الموجودة [Office؟](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**ملاحظة:** إذا كنت لا تريد الانتظار حتى جدول النشر هذا، يمكنك نشر Teams كملف مستقل [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)للمستخدمين باتباع هذه الإرشادات، أو يمكنك أن تقوم بتثبيت المستخدمين Teams لأنفسهم من https://teams.microsoft.com/downloads .

إذا لم تكن مؤسستك جاهزة لنشر Teams، يمكنك استبعاد Teams [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) من [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) عمليات تثبيت جديدة أو موجودة Office.  إذا كنت Teams تثبيته، ولكنك لا تريد أن يبدأ Teams تلقائيا للمستخدم بعد تثبيته، فشاهد منع بدء Microsoft Teams تلقائيا بعد [التثبيت](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

***إلغاء تثبيت Teams*** من جهاز يعمل Windows، راجع إلغاء [تثبيت](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81)Microsoft Teams . لتنظيف Microsoft Teams من أجهزة أو مستخدمين هدفين متعددين، راجع Microsoft Teams [النشر.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

إذا كنت تستخدم أجهزة كمبيوتر مشتركة أو خدمات سطح المكتب البعيد (RDS) أو البنية الأساسية لسطح المكتب الظاهري (VDI)، فشاهد بيئات [VDI والكمبيوتر](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)المشترك مع Microsoft Teams. إذا كنت تستخدم Office for Mac، فشاهد Microsoft Teams [التثبيتات على جهاز Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**ملاحظة:** بعد Teams تثبيت التطبيق، يتم [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) تحديثه تلقائيا كل أسبوعين تقريبا بالميزات الجديدة وتحديثات الجودة. 