---
title: تمكين Office 365 ATP SharePoint OneDrive و Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 61ca448ef146f3f6fb930f0dc6f09f41bde72087f56ffba820f0a2d517cddb31
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53964620"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>تمكين Microsoft Defender Office 365 SharePoint عبر الإنترنت OneDrive و Microsoft Teams

1. انتقل إلى https://protection.office.com ثم سجل الدخول.
2. اختر **نهج إدارة** المخاطر  >  **خزينة**  >  **المرفقات**.
3. حدد **تشغيل Defender Office 365 SharePoint** OneDrive و Microsoft Teams ، ثم انقر فوق **حفظ**.
4. (مستحسن) كمسؤول عام أو مسؤول SharePoint Online، قم بتشغيل الأمر [Cmdlet Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) مع تعيين المعلمة **DisallowInfectedFileDownload** إلى *true*.
5. (مستحسن) [إعداد التنبيهات](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) للملفات التي تم الكشف عنها.

> [!NOTE]
> لن يقوم Microsoft Defender Office 365 بفحص كل ملف في SharePoint أو OneDrive أو Microsoft Teams. يتم فحص الملفات بشكل غير متزامن، من خلال عملية تستخدم أحداث نشاط الضيف والمشاركة، إلى جانب مؤشرات بحث ذكية وإشارات تهديدات لتحديد الملفات الضارة. راجع [Microsoft Defender Office 365 SharePoint OneDrive و Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).