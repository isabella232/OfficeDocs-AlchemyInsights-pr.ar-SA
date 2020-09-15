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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709894"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>تمكين الحماية المتقدمة من المخاطر ل Office 365 لفرق SharePoint Online و OneDrive و Microsoft

1. انتقل إلى https://protection.office.com وسجل الدخول.
2. اختر **Threat management**  >  **Policy**  >  **المرفقات الامنه**لنهج أداره المخاطر.
3. حدد **تشغيل ATP لفرق SharePoint و OneDrive و Microsoft**، ثم انقر فوق **حفظ**.
4. مطلوب بصفتك مسؤولا عاما أو مسؤول SharePoint Online ، قم بتشغيل الأمر cmdlet [سبوتينانت](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) مع تعيين المعلمة **ديسالووينفيكتيدفيليدوونلواد** إلى *true*.
5. مطلوب [اعداد التنبيات](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) للملفات التي تم الكشف عنها.

> [!NOTE]
> سيقوم ATP بفحص كل ملف واحد في SharePoint Online أو OneDrive أو فرق Microsoft. يتم مسح الملفات بشكل غير متزامن ، من خلال عمليه تستخدم احداث نشاط المشاركة والضيف ، إلى جانب المعرفات الذكية وإشارات التهديد لتحديد الملفات الضارة. راجع [ATP لفرق SharePoint و OneDrive و Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).