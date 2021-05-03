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
# <a name="troubleshooting-import-service-job-stuck"></a>مهمة "خدمة الاستيراد" التي تم استكشافها وإصلاحها عالقة

إذا كنت تواجه مشاكل تتعلق باستيراد مهام الخدمة عالقة أو معلقة، فجرب ما يلي:

- راجع حجم ملف PST. الحد الأقصى الموصى به لحجم ملف PST لاستيراده هو 20 غيغابايت.

- إذا كنت تشك في العناصر التي تم تخطيها بسبب تلف، Scanpst.exe على تشخيص الأخطاء في ملفات PST وإصلاحها.

- إذا ظهر الخطأ "MapiExceptionShutoffQuotaExceeded" أثناء الاستيراد، فتأكد من أن علبة البريد الهدف لديها سعة كافية لاستيراد ملفات PST المطلوبة.

لمزيد من المعلومات حول استكشاف مشاكل مهمة استيراد PST وإصلاحها، راجع استكشاف المشاكل المتعلقة ب مهام [استيراد PST وإصلاحها](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

للحصول على معلومات حول كيفية إصلاح المشاكل عند استيراد PSTs إلى Outlook، راجع إصلاح المشاكل المتعلقة باستيراد ملف pst Outlook [pst (microsoft.com).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)