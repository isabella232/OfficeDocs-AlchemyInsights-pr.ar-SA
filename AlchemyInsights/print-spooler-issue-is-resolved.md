---
title: تم حل مشكلة التخزين المؤقت للطباعة
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088273"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="d01b2-102">تم حل مشكلة التخزين المؤقت للطباعة</span><span class="sxs-lookup"><span data-stu-id="d01b2-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="d01b2-103">إذا تم تحديث الجهاز باستخدام Windows 10 **OS Build 19041.329**، فقد تكون قد لاحظت مشكلة حيث تفشل بعض الطابعات في الطباعة.</span><span class="sxs-lookup"><span data-stu-id="d01b2-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="d01b2-104">قد يؤدي التخزين المؤقت للطباعة إلى إلقاء خطأ أو إغلاقه بشكل غير متوقع عند محاولة الطباعة، ولا يأتي أي إخراج من الطابعة المتأثرة.</span><span class="sxs-lookup"><span data-stu-id="d01b2-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="d01b2-105">يتم حل هذه المشكلة في نظام التشغيل **19041.331**بناء ، [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="d01b2-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="d01b2-106">**التحقيق الجاري**</span><span class="sxs-lookup"><span data-stu-id="d01b2-106">**Ongoing investigation**</span></span>

<span data-ttu-id="d01b2-107">قد يفشل ملف خدمة النظام الفرعي لـ "المرجع الأمان المحلي" (LSASS)\*\* (Isass.exe) \*\*على بعض الأجهزة التي بها رسالة الخطأ، "فشلت عملية نظام حرجة، C:\WINDOWS\system32\Isass.exe، مع رمز الحالة c000008.</span><span class="sxs-lookup"><span data-stu-id="d01b2-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="d01b2-108">يجب الآن إعادة تشغيل الجهاز".</span><span class="sxs-lookup"><span data-stu-id="d01b2-108">The machine must now be restarted".</span></span>  <span data-ttu-id="d01b2-109">**تعمل Microsoft على حل وستوفر تحديثًا في إصدار قادم.**</span><span class="sxs-lookup"><span data-stu-id="d01b2-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="d01b2-110">لمزيد من المعلومات، يرجى مراجعة [Windows 10 الإصدار 2004 المشكلات المعروفة](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="d01b2-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>