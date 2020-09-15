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
# <a name="print-spooler-issue-is-resolved"></a>تم حل مشكله المخزن المؤقت للطباعة

إذا تم تحديث جهازك باستخدام Windows 10  **OS الإصدار 19041.329**، فمن المحتمل انك قد بدات بالمشكلة عند فشل طباعه بعض الطابعات. قد يؤدي التخزين المؤقت للطباعة إلى طرح خطا أو إغلاق بشكل غير متوقع عند محاولة الطباعة ، ولا ياتي اي إخراج من الطابعة المتاثره. تم حل هذه المشكلة في نظام التشغيل OS  **19041.331** [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**استقصاء مستمر**

قد يفشل ملف نظام التشغيل الفرعي لتخويل الأمان المحلي (LSASS) (**Isass.exe**) علي بعض الاجهزه التي تحتوي علي رسالة الخطا ، "عمليه النظام الهامه ، الC:\WINDOWS\system32\Isass.exe ، فشل مع c0000008 رمز الحالة. يجب أعاده تشغيل الجهاز الآن ".  **تعمل Microsoft بدقه ستوفر تحديثا في إصدار قادم.**

لمزيد من المعلومات ، يرجى الاطلاع علي  [المشاكل المعروفة في 2004 إصدار Windows 10](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).