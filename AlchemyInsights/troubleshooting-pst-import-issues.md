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
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="6d6dc-102">استكشاف مشاكل استيراد PST وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="6d6dc-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="6d6dc-103">إذا كنت تقوم باستيراد ملف داخل عميل Outlook نفسه، فشاهد إصلاح المشاكل المتعلقة باستيراد [ملف pst. في Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="6d6dc-103">If you are importing within the Outlook client itself, see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="6d6dc-104">إذا كنت تستخدم خدمة الاستيراد وتعثرت، فلاحظ أن كل ملف PST تقوم بتحميله إلى موقع تخزين Azure يجب ألا يزيد عن 20 غيغابايت.</span><span class="sxs-lookup"><span data-stu-id="6d6dc-104">If you are using Import Service and it's stuck, note that each PST file that you upload to the Azure Storage location should be no larger than 20GB.</span></span> <span data-ttu-id="6d6dc-105">قد تؤثر ملفات PST التي يزيد حجمها عن 20 غيغابايت على أداء عملية استيراد PST.</span><span class="sxs-lookup"><span data-stu-id="6d6dc-105">PST files larger than 20GB may impact the performance of the PST import process.</span></span> <span data-ttu-id="6d6dc-106">لمزيد من المعلومات حول استكشاف المهام العالقة وإصلاحها، راجع المشاكل [التي تؤثر على مهام استيراد PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="6d6dc-106">For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

- <span data-ttu-id="6d6dc-107">إذا كنت تريد التحقق من حالة مهمة استيراد معينة، فاستخدم [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="6d6dc-107">If you want to verify the status of a specific Import job, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="6d6dc-108">للحصول على التفاصيل الكاملة حول خدمة الاستيراد، راجع نظرة عامة حول استيراد ملفات PST الخاصة [بالمنظمة](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="6d6dc-108">For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
