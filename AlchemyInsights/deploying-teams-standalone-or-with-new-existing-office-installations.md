---
title: نشر أفرقة مستقلة أو مع عمليات تثبيت Office جديد أو موجود
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054218"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>نشر أفرقة مستقلة أو مع عمليات تثبيت Office جديد أو موجود

الفرق Microsoft الآن مدرجة كجزء من ***عمليات التثبيت الجديدة*** من Office 365 ProPlus Office 365 الأعمال ومكتب لجنة الهدنة العسكرية. لمزيد من المعلومات، راجع [عندما فرق Microsoft ستبدأ يتم تضمينها مع عمليات تثبيت جديد ل Office؟](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

بالإضافة إلى ذلك، بدءاً من الإصدار 1906 في القناة شهريا، الفرق سيكون ***إضافة إلى المنشآت القائمة*** Office 365 ProPlus (ومكتب الأعمال 365) على أجهزة تشغيل Windows عند تحديث تثبيت موجود للإصدار الأحدث. لمزيد من المعلومات، راجع [ما حول المنشآت القائمة من Office؟](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> إذا لم ترغب في الانتظار لجدولة هذه العملية التمهيدية، يمكنك نشر فرق كمستقل للمستخدمين [اتباع هذه الإرشادات](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) أو يمكنك جعل المستخدمين تثبيت الفرق لأنفسهم من [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

إذا لم يكن مؤسستك جاهزة لنشر أفرقة، لدينا على الخطوات التي يمكنك اتخاذها ***استبعاد الفرق*** من منشآت [جديدة](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) أو [موجودة](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) من Office. إذا كنت تريد الفرق بتثبيت، ولكن لا تريد الفرق ليتم تشغيله تلقائياً للمستخدم بعد تثبيته، راجع [منع Microsoft فرق من بدء التشغيل تلقائياً بعد التثبيت](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

***إلغاء تثبيت فرق*** من جهاز يقوم بتشغيل Windows، راجع [إزالة تثبيت Microsoft الفرق](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). لتنظيف فرق Microsoft من المستخدمين أو الأجهزة الهدف متعددة، راجع [مسح نشر فرق Microsoft](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

إذا كنت تستخدم أجهزة الكمبيوتر المشتركة أو خدمات سطح المكتب البعيد (RDS) "البنية التحتية" سطح المكتب الظاهري (VDI)، راجع [الكمبيوتر المشتركة وبيئات VDI مع فرق Microsoft](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

إذا كنت تستخدم Macلنظام التشغيل Office، راجع [تثبيت Microsoft الفرق في نظام التشغيل Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> بعد تثبيت الفرق من [تحديثه تلقائياً](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) كل أسبوعين تقريبا مع الميزات الجديدة والتحديثات الجودة. 