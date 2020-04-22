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
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703413"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>تمكين Office 365 حماية متقدمة من التهديدات لفرق SharePoint Online وOneDrive وMicrosoft

1. اذهب https://protection.office.com إلى وتسجيل الدخول.
2. اختر**مرفقات****آمنة لسياسة** >  **إدارة** > التهديدات.
3. حدد **تشغيل ATP لـ SharePoint و OneDrive وفرق Microsoft**، ثم انقر فوق **حفظ**.
4. (موصى به) كمسؤول عمومي أو مسؤول SharePoint عبر الإنترنت، قم بتشغيل [cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) مع تعيين معلمة **FileFileDownload غير مسموح** بها إلى *صواب*.
5. (موصى به) [إعداد تنبيهات](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) للملفات التي تم اكتشافها.

> [!NOTE]
> سوف ATP nto مسح كل ملف واحد في SharePoint عبر الإنترنت أو OneDrive أو Microsoft Teams. يتم مسح الملفات ضوئيًا بشكل غير متزامن، من خلال عملية تستخدم أحداث المشاركة وأحداث نشاط الضيف، بالإضافة إلى الاستدلالات الذكية وإشارات التهديد لتحديد الملفات الضارة. راجع [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).