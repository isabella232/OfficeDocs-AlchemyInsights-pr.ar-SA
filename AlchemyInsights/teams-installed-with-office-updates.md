---
title: فرق مثبته مع تحديثات Office
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
- "2599"
- "9000140"
- "9000660"
- "2509"
ms.openlocfilehash: 9a09800fcc36876629c7d59182f20b5b16393ef8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47736491"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>فرق Microsoft المثبتة مع تحديثات Office

يتم تضمين فرق Microsoft كجزء من ***عمليات التثبيت الجديدة*** لتطبيقات microsoft 365 ل Enterprise و Microsoft 365 apps for Business و Office for Mac. لمزيد من المعلومات ، راجع [متى ستبدا فرق Microsoft في التضمين في عمليات التثبيت الجديدة ل Office ؟](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

بالاضافه إلى ذلك ، بدءا من الإصدار 1906 في القناة الحالية ، ستتم أضافه الفرق تدريجيا إلى ***عمليات التثبيت الموجودة*** لتطبيقات Microsoft 365 للمؤسسة (وتطبيقات microsoft 365 for business) علي الاجهزه التي تعمل بنظام التشغيل Windows عند تحديث التثبيت الحالي إلى الإصدار الأخير. لمزيد من المعلومات ، راجع [ماذا عن التثبيتات الموجودة في Office ؟](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**ملاحظه:** إذا كنت لا تريد الانتظار لجدول التمهيد هذا ، يمكنك نشر الفرق كمستقلين للمستخدمين عن طريق [اتباع الإرشادات التالية](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)، أو يمكنك جعل المستخدمين يقومون بتثبيت الفرق لأنفسهم https://teams.microsoft.com/downloads .

إذا لم تكن مؤسستك جاهزه لنشر الفرق ، يمكنك ***استبعاد الفرق*** من تثبيتات Office [الجديدة](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) أو [الموجودة](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) . إذا كنت تريد تثبيت الفرق ، ولكنك لا تريد ان تبدا الفرق تلقائيا للمستخدم بعد تثبيته ، فراجع [منع فرق Microsoft من بدء التشغيل تلقائيا بعد التثبيت](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

***للغاء تثبيت الفرق*** من جهاز يقوم بتشغيل Windows ، راجع [أزاله تثبيت فرق Microsoft](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81). لتنظيف فرق Microsoft من الاجهزه المستهدفة أو المستخدمين المتعددين ، راجع [تنظيف نشر الفرق في Microsoft](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

إذا كنت تستخدم أجهزه الكمبيوتر المشتركة أو خدمات سطح المكتب البعيد (RDS) أو البنية الاساسيه لسطح المكتب الظاهري (VDI) ، فراجع [بيئات الكمبيوتر المشتركة والVDI مع فرق Microsoft](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams). إذا كنت تستخدم Office for Mac ، فراجع [تثبيتات فرق Microsoft علي جهاز Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**ملاحظه:** بعد تثبيت الفرق ، يتم [تحديثها تلقائيا](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) كل أسبوعين تقريبا باستخدام الميزات الجديدة وتحديثات الجودة. 