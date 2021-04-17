---
title: Teams مثبت مع تحديثات Office
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
ms.openlocfilehash: 36b0b1a7bf37c27304b4124157dba9aba337678c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832369"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>Microsoft Teams مثبت مع تحديثات Office

يتم تضمين Microsoft Teams  كجزء من عمليات التثبيت الجديدة لتطبيقات Microsoft 365 للمؤسسات وتطبيقات Microsoft 365 للأعمال Macلنظام التشغيل Office. لمزيد من المعلومات، [راجع متى سيبدأ تضمين Microsoft Teams مع عمليات التثبيت الجديدة ل Office؟](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

بالإضافة إلى ذلك، بدءا من الإصدار 1906 في التحديث  الحالي، سيتم إضافة Teams تدريجيا إلى عمليات التثبيت الموجودة لتطبيقات Microsoft 365 للمؤسسات (وتطبيقات Microsoft 365 للأعمال) على الأجهزة التي تعمل بنظام التشغيل Windows عند تحديث التثبيت الحالي إلى الإصدار الأخير. لمزيد من المعلومات، راجع [ماذا عن عمليات تثبيت Office الموجودة؟](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**ملاحظة:** إذا كنت لا تريد الانتظار حتى جدول النشر هذا، يمكنك نشر Teams كملف مستقل للمستخدمين باتباع هذه الإرشادات، أو يمكنك أن يقوم المستخدمون بتثبيت Teams لأنفسهم من [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) https://teams.microsoft.com/downloads .

إذا لم تكن مؤسستك جاهزة لنشر Teams، يمكنك [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) استبعاد ***Teams*** من عمليات تثبيت Office الجديدة [أو](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) الموجودة. إذا كنت تريد تثبيت Teams، ولكنك لا تريد أن يبدأ Teams تلقائيا للمستخدم بعد تثبيته، فشاهد منع [بدء تشغيل Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)تلقائيا بعد التثبيت .

***إلغاء تثبيت Teams*** من جهاز يعمل بنظام التشغيل Windows، راجع إلغاء تثبيت Microsoft [Teams](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81). لتنظيف Microsoft Teams من أجهزة أو مستخدمين هدفين متعددين، راجع [تنظيف نشر Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

إذا كنت تستخدم أجهزة كمبيوتر مشتركة أو خدمات سطح المكتب البعيد (RDS) أو البنية الأساسية لسطح المكتب الظاهري (VDI)، فشاهد بيئات [VDI](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)والكمبيوتر المشترك مع Microsoft Teams . إذا كنت تستخدم Macلنظام التشغيل Office، فشاهد عمليات تثبيت [Microsoft Teams على جهاز Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**ملاحظة:** بعد تثبيت Teams، يتم [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) تحديثه تلقائيا كل أسبوعين تقريبا بالميزات الجديدة وتحديثات الجودة. 