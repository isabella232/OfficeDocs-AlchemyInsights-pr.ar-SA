---
title: تمكين Office 365 ATP لفرق SharePoint و OneDrive و Microsoft
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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801034"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>تمكين Microsoft Defender ل Office 365 for SharePoint Online و OneDrive و Microsoft

1. انتقل إلى https://protection.office.com وسجل الدخول.
2. اختر **Threat management**  >  **Policy**  >  **المرفقات الامنه** لنهج أداره المخاطر.
3. حدد **تشغيل ATP لفرق SharePoint و OneDrive و Microsoft** ، ثم انقر فوق **حفظ** .
4. مطلوب بصفتك مسؤولا عاما أو مسؤول SharePoint Online ، قم بتشغيل الأمر cmdlet [سبوتينانت](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) مع تعيين المعلمة **ديسالووينفيكتيدفيليدوونلواد** إلى *true* .
5. مطلوب [اعداد التنبيات](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) للملفات التي تم الكشف عنها.

> [!NOTE]
> سيقوم ATP بفحص كل ملف واحد في SharePoint Online أو OneDrive أو فرق Microsoft. يتم مسح الملفات بشكل غير متزامن ، من خلال عمليه تستخدم احداث نشاط المشاركة والضيف ، إلى جانب المعرفات الذكية وإشارات التهديد لتحديد الملفات الضارة. راجع [ATP لفرق SharePoint و OneDrive و Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).