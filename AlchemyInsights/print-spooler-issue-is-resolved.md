---
title: تم حل مشكله المخزن المؤقت للطباعة
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801828"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="2add7-102">تم حل مشكله المخزن المؤقت للطباعة</span><span class="sxs-lookup"><span data-stu-id="2add7-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="2add7-103">إذا تم تحديث جهازك باستخدام Windows 10  **OS الإصدار 19041.329**، فمن المحتمل انك قد بدات بالمشكلة عند فشل طباعه بعض الطابعات.</span><span class="sxs-lookup"><span data-stu-id="2add7-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="2add7-104">قد يؤدي التخزين المؤقت للطباعة إلى طرح خطا أو إغلاق بشكل غير متوقع عند محاولة الطباعة ، ولا ياتي اي إخراج من الطابعة المتاثره.</span><span class="sxs-lookup"><span data-stu-id="2add7-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="2add7-105">تم حل هذه المشكلة في نظام التشغيل OS  **19041.331** [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="2add7-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="2add7-106">**استقصاء مستمر**</span><span class="sxs-lookup"><span data-stu-id="2add7-106">**Ongoing investigation**</span></span>

<span data-ttu-id="2add7-107">قد يفشل ملف نظام التشغيل الفرعي لتخويل الأمان المحلي (LSASS) (**Isass.exe**) علي بعض الاجهزه التي تحتوي علي رسالة الخطا ، "عمليه النظام الهامه ، الC:\WINDOWS\system32\Isass.exe ، فشل مع c0000008 رمز الحالة.</span><span class="sxs-lookup"><span data-stu-id="2add7-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="2add7-108">يجب أعاده تشغيل الجهاز الآن ".</span><span class="sxs-lookup"><span data-stu-id="2add7-108">The machine must now be restarted".</span></span>  <span data-ttu-id="2add7-109">**تعمل Microsoft بدقه ستوفر تحديثا في إصدار قادم.**</span><span class="sxs-lookup"><span data-stu-id="2add7-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="2add7-110">لمزيد من المعلومات ، يرجى الاطلاع علي  [المشاكل المعروفة في 2004 إصدار Windows 10](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="2add7-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>