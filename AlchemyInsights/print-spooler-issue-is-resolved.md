---
title: تم حل مشكلة "ا spooler الطباعة"
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
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911325"
---
# <a name="print-spooler-issue-is-resolved"></a>تم حل مشكلة "ا spooler الطباعة"

إذا تم تحديث جهازك باستخدام Windows 10  **OS Build 19041.329**، فقد تكون لاحظت مشكلة في فشل بعض الطابعات في الطباعة. قد تقوم مجموعة مواخير الطباعة برمي رسالة خطأ أو إغلاقها بشكل غير متوقع عند محاولة الطباعة، ولا يتم الحصول على أي إخراج من الطابعة المتأثرة. يتم حل هذه المشكلة في إصدار نظام التشغيل  **19041.331**، [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**التحقيق الجاري**

قد يفشل ملف خدمة النظام الفرعي (LSASS) الخاص بهيئة الأمان المحلية **(Isass.exe)** على بعض الأجهزة التي تظهر فيها رسالة الخطأ "فشلت عملية النظام الهامة، C:\WINDOWS\system32\Isass.exe، مع رمز الحالة c0000008. يجب إعادة تشغيل الجهاز الآن".  **تعمل Microsoft على حل وستوفر تحديثا في إصدار قادم.**

لمزيد من المعلومات، يرجى الاطلاع على المشاكل المعروفة في  [إصدار 2004 من Windows 10](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).