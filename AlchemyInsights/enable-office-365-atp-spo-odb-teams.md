---
title: تمكين Office 365 ATP لفرق SharePoint وOneDrive وMicrosoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506905"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>تمكين Office 365 حماية متقدمة من التهديدات لفرق SharePoint Online وOneDrive وMicrosoft

1. اذهب إلى https://protection.office.com وتسجيل الدخول.
2. اختر **Threat management**  >  مرفقات آمنة لسياسة**إدارة**  >  **Safe Attachments**التهديدات.
3. حدد **تشغيل ATP لـ SharePoint و OneDrive وفرق Microsoft**، ثم انقر فوق **حفظ**.
4. (موصى به) كمسؤول عمومي أو مسؤول SharePoint عبر الإنترنت، قم بتشغيل [cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) مع تعيين معلمة **FileFileDownload غير مسموح** بها إلى *صواب*.
5. (موصى به) [إعداد تنبيهات](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) للملفات التي تم اكتشافها.

> [!NOTE]
> سوف ATP nto مسح كل ملف واحد في SharePoint عبر الإنترنت أو OneDrive أو Microsoft Teams. يتم مسح الملفات ضوئيًا بشكل غير متزامن، من خلال عملية تستخدم أحداث المشاركة وأحداث نشاط الضيف، بالإضافة إلى الاستدلالات الذكية وإشارات التهديد لتحديد الملفات الضارة. راجع [ATP لـ SharePoint و OneDrive وفرق Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).