---
title: تمكين خزينة المرفقات SharePoint عبر الإنترنت OneDrive Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332366"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>تمكين خزينة المرفقات SharePoint عبر الإنترنت OneDrive Microsoft Teams

1. باستخدام بيانات اعتماد المسؤول العام أو مسؤول الأمان، افتح مدخل Microsoft 365 Defender في ، ثم انتقل إلى سياسات & قواعد المخاطر خزينة <https://security.microsoft.com>  \>  \> **المرفقات**  في القسم "سياسات"

   الانتقال مباشرة إلى صفحة المرفقات **خزينة،** استخدم <https://security.microsoft.com/safeattachmentv2> .

2. في صفحة **خزينة المرفقات،** انقر فوق **إعدادات عام**.
3. في flyout التي تظهر، حدد **تشغيل Microsoft Defender ل** Office 365 ل SharePoint OneDrive و Microsoft Teams ، ثم حدد **حفظ**.

    **تلميح**: قم بالخطوات التالية لتحسين حماية خزينة المرفقات SharePoint OneDrive Microsoft Teams:
    - لمنع المستخدمين من تنزيل الملفات الضارة، استخدم قيمة المعلمة `$true` *DisallowInfectedFileDownload* على الأمر **[cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** في SharePoint Online PowerShell. لمزيد من المعلومات، راجع [استخدام SharePoint Online PowerShell](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)لمنع المستخدمين من تنزيل ملفات ضارة .
    - [إنشاء نهج تنبيه للملفات التي تم الكشف عنها](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

لمزيد من المعلومات، راجع خزينة [المرفقات Office 365 SharePoint](https://go.microsoft.com/fwlink/?linkid=2092041)OneDrive Microsoft Teams .
