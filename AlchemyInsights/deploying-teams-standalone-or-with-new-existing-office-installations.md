---
title: نشر الفرق كوحدة مستقلة أو مع عمليات تثبيت Office جديدة أو موجودة
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: ffa91eaf333792af149feda25f9a377ed591b597
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010205"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>نشر الفرق كوحدة مستقلة أو مع عمليات تثبيت Office جديدة أو موجودة

يتم الآن تضمين Microsoft Teams كجزء من ***عمليات التثبيت الجديدة*** لتطبيقات Microsoft 365 للمؤسسات وMicrosoft 365 Apps للأعمال وOffice for Mac. لمزيد من المعلومات، راجع [متى سيتم تضمين Microsoft Teams مع عمليات التثبيت الجديدة من Office؟](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

بالإضافة إلى ذلك، بدءًا من الإصدار 1906 في القناة الشهرية، ستتم إضافة الفرق ***إلى عمليات التثبيت الحالية*** لتطبيقات Microsoft 365 للمؤسسات (وMicrosoft 365 Apps for business) على الأجهزة التي تعمل بنظام التشغيل Windows عند تحديث التثبيت الحالي إلى أحدث إصدار. لمزيد من المعلومات، راجع [ماذا عن عمليات التثبيت الحالية لـ Office؟](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> إذا كنت لا تريد الانتظار لهذا الجدول التمهيدي، يمكنك نشر Teams كمستقل للمستخدمين باتباع [هذه الإرشادات](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) أو يمكنك [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)أن تدع المستخدمين يقومون بتثبيت Teams لأنفسهم من .

إذا لم تكن مؤسستك مستعدة لنشر Teams، فلدينا الخطوات التي يمكنك اتخاذها ***لاستبعاد الفرق*** من عمليات التثبيت [الجديدة](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) أو [الحالية](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) في Office. إذا كنت تريد تثبيت الفرق، ولكنك لا تريد أن تبدأ الفرق تلقائيًا للمستخدم بعد تثبيته، فراجع [منع Microsoft Teams من البدء تلقائيًا بعد التثبيت](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

***لإلغاء تثبيت "الفرق"*** من جهاز يعمل بنظام التشغيل Windows، راجع [إلغاء تثبيت "فرق Microsoft".](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) لتنظيف Microsoft Teams من أجهزة أو مستخدمين مستهدفين متعددة، راجع [تنظيف نشر Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

إذا كنت تستخدم أجهزة كمبيوتر مشتركة أو خدمات سطح المكتب البعيد (RDS) أو البنية التحتية لسطح المكتب الظاهري (VDI)، فراجع [بيئات الكمبيوتر المشتركة وبيئات VDI مع Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

إذا كنت تستخدم Office for Mac، فراجع [عمليات تثبيت Microsoft Teams على Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> بعد تثبيت Teams، يتم [تحديثه تلقائيًا](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) كل أسبوعين تقريبًا باستخدام ميزات جديدة وتحديثات عالية الجودة. 