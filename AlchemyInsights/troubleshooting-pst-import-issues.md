---
title: استكشاف مشاكل استيراد PST وإصلاحها
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059802"
---
# <a name="troubleshooting-pst-import-issues"></a>استكشاف مشاكل استيراد PST وإصلاحها

- إذا كنت تقوم باستيراد ملف داخل عميل Outlook نفسه، فشاهد إصلاح المشاكل المتعلقة باستيراد [ملف pst. في Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- إذا كنت تستخدم خدمة الاستيراد وتعثرت، فلاحظ أن كل ملف PST تقوم بتحميله إلى موقع تخزين Azure يجب ألا يزيد عن 20 غيغابايت. قد تؤثر ملفات PST التي يزيد حجمها عن 20 غيغابايت على أداء عملية استيراد PST. لمزيد من المعلومات حول استكشاف المهام العالقة وإصلاحها، راجع المشاكل [التي تؤثر على مهام استيراد PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- إذا كنت تريد التحقق من حالة مهمة استيراد معينة، فاستخدم [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- للحصول على التفاصيل الكاملة حول خدمة الاستيراد، راجع نظرة عامة حول استيراد ملفات PST الخاصة [بالمنظمة](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
