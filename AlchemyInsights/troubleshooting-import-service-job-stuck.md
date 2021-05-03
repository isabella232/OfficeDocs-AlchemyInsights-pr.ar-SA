---
title: مهمة "خدمة الاستيراد" التي تم استكشافها وإصلاحها عالقة
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2021
ms.locfileid: "52124748"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="f3e3f-102">مهمة "خدمة الاستيراد" التي تم استكشافها وإصلاحها عالقة</span><span class="sxs-lookup"><span data-stu-id="f3e3f-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="f3e3f-103">إذا كنت تواجه مشاكل تتعلق باستيراد مهام الخدمة عالقة أو معلقة، فجرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="f3e3f-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="f3e3f-104">راجع حجم ملف PST.</span><span class="sxs-lookup"><span data-stu-id="f3e3f-104">Review the size of of the PST file.</span></span> <span data-ttu-id="f3e3f-105">الحد الأقصى الموصى به لحجم ملف PST لاستيراده هو 20 غيغابايت.</span><span class="sxs-lookup"><span data-stu-id="f3e3f-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="f3e3f-106">إذا كنت تشك في العناصر التي تم تخطيها بسبب تلف، Scanpst.exe على تشخيص الأخطاء في ملفات PST وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="f3e3f-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="f3e3f-107">إذا ظهر الخطأ "MapiExceptionShutoffQuotaExceeded" أثناء الاستيراد، فتأكد من أن علبة البريد الهدف لديها سعة كافية لاستيراد ملفات PST المطلوبة.</span><span class="sxs-lookup"><span data-stu-id="f3e3f-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="f3e3f-108">لمزيد من المعلومات حول استكشاف مشاكل مهمة استيراد PST وإصلاحها، راجع استكشاف المشاكل المتعلقة ب مهام [استيراد PST وإصلاحها](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="f3e3f-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="f3e3f-109">للحصول على معلومات حول كيفية إصلاح المشاكل عند استيراد PSTs إلى Outlook، راجع إصلاح المشاكل المتعلقة باستيراد ملف pst Outlook [pst (microsoft.com).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)</span><span class="sxs-lookup"><span data-stu-id="f3e3f-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>