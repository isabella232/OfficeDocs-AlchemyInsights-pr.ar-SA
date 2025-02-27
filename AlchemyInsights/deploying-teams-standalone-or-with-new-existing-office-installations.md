---
title: نشر Teams مستقلة أو مع عمليات تثبيت Office موجودة
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320109"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>نشر Teams مستقلة أو مع عمليات تثبيت Office موجودة

Microsoft Teams الآن كجزء من عمليات  التثبيت الجديدة Microsoft 365 Apps for enterprise Microsoft 365 Apps for business Office for Mac. لمزيد من المعلومات، راجع [متى Microsoft Teams يتم تضمينه](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps) مع عمليات التثبيت الجديدة Office؟

بالإضافة إلى ذلك، بدءا من الإصدار 1906 في التحديث  الحالي، سيضاف Teams إلى عمليات التثبيت الموجودة ل Microsoft 365 Apps for enterprise (و Microsoft 365 Apps for business) على الأجهزة التي تعمل Windows عند تحديث التثبيت الموجود إلى الإصدار الأخير. لمزيد من المعلومات، راجع ماذا عن عمليات التثبيت الموجودة [Office؟](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**ملاحظة:** إذا كنت لا تريد الانتظار حتى جدول النشر هذا، يمكنك نشر Teams كملف [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) مستقل للمستخدمين باتباع هذه الإرشادات أو يمكنك أن يقوم المستخدمون بتثبيت Teams لأنفسهم من [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

إذا لم تكن مؤسستك جاهزة لنشر Teams، لدينا الخطوات التي يمكنك اتخاذها ***لاستبعاد*** Teams [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) من عمليات التثبيت الجديدة أو الموجودة Office. [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) إذا كنت Teams تثبيته، ولكنك لا تريد أن Teams تلقائيا للمستخدم بعد تثبيته، فشاهد منع بدء Microsoft Teams تلقائيا بعد [التثبيت](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

***إلغاء تثبيت Teams*** من جهاز يعمل Windows، راجع إلغاء [تثبيت](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)Microsoft Teams . لتنظيف Microsoft Teams من أجهزة أو مستخدمين هدفين متعددين، راجع Microsoft Teams [تنظيف النشر.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

إذا كنت تستخدم أجهزة كمبيوتر مشتركة أو خدمات سطح المكتب البعيد (RDS) أو البنية الأساسية لسطح المكتب الظاهري (VDI)، فشاهد بيئات [VDI والكمبيوتر](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)المشترك مع Microsoft Teams .

إذا كنت تستخدم Office for Mac، فشاهد Microsoft Teams [التثبيتات على جهاز Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**ملاحظة:** بعد Teams تثبيت التطبيق، يتم [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) تحديثه تلقائيا كل أسبوعين تقريبا بالميزات الجديدة وتحديثات الجودة. 