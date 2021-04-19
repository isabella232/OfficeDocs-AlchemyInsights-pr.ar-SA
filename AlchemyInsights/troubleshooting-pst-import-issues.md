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
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826150"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="7bfb3-102">استكشاف مشاكل استيراد PST وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="7bfb3-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="7bfb3-103">في حالة الاستيراد ضمن عميل Outlook ذاته، يرجى الاطلاع على [تصحيح المشاكل عند استيراد ملف .pst في Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="7bfb3-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="7bfb3-104">إذا تم تعليق «خدمة الاستيراد» أثناء استخدامها، فيرجى العلم أن كل ملف PST تحمله إلى موقع «تخزين Azure» يجب ألا يتجاوز حجمه 20 GB.</span><span class="sxs-lookup"><span data-stu-id="7bfb3-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="7bfb3-105">قد تؤثر ملفات PST التي يتجاوز حجمها عن 20 GB على أداء عمليه استيراد PST.</span><span class="sxs-lookup"><span data-stu-id="7bfb3-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="7bfb3-106">إذا كنت تريد التحقق من حالة مهمة استيراد معينة، فيمكنك استخدام [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="7bfb3-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="7bfb3-107">لمعرفة التفاصيل الكاملة حول خدمة الاستيراد، يرجى الاطلاع على [نظرة عامة حول استيراد ملفات PST لمؤسستك](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="7bfb3-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
