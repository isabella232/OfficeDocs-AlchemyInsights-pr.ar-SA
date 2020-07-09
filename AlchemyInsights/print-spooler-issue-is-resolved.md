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
# <a name="print-spooler-issue-is-resolved"></a>تم حل مشكلة التخزين المؤقت للطباعة

إذا تم تحديث الجهاز باستخدام Windows 10 **OS Build 19041.329**، فقد تكون قد لاحظت مشكلة حيث تفشل بعض الطابعات في الطباعة. قد يؤدي التخزين المؤقت للطباعة إلى إلقاء خطأ أو إغلاقه بشكل غير متوقع عند محاولة الطباعة، ولا يأتي أي إخراج من الطابعة المتأثرة. يتم حل هذه المشكلة في نظام التشغيل **19041.331**بناء ، [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**التحقيق الجاري**

قد يفشل ملف خدمة النظام الفرعي لـ "المرجع الأمان المحلي" (LSASS)** (Isass.exe) **على بعض الأجهزة التي بها رسالة الخطأ، "فشلت عملية نظام حرجة، C:\WINDOWS\system32\Isass.exe، مع رمز الحالة c000008. يجب الآن إعادة تشغيل الجهاز".  **تعمل Microsoft على حل وستوفر تحديثًا في إصدار قادم.**

لمزيد من المعلومات، يرجى مراجعة [Windows 10 الإصدار 2004 المشكلات المعروفة](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).