---
title: أداة تشخيص الخدمة لسطح المكتب الظاهري ل Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595425"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>أداة تشخيص الخدمة لسطح المكتب الظاهري ل Windows

يوفر Windows Virtual Desktop (WVD) أداة تشخيص تسمح للمسؤولين بتحديد الأخطاء من خلال واجهة واحدة. تقوم هذه الأداة بتسجيل المعلومات ذات الصلة بالت تشخيص كلما تم استخدام WVD من قبل شخص تم تعيين دور WVD له. يحتوي كل سجل على معلومات حول دور WVD الذي يتضمنه النشاط، ورسائل الخطأ التي تظهر أثناء جلسة العمل، ومعلومات حول المستأجر والمستخدم. يمكن تكوين Azure Log Analytics لتسجيل سجل النشاط الذي أنشأته أداة التشخيص باتباع الخطوات التالية:

1. إنشاء مساحة عمل Log Analytics باستخدام [مدخل Azure](https://go.microsoft.com/fwlink/?linkid=2129500) أو [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).

1. [توصيل أجهزة كمبيوتر Windows ب Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). احصل على "مفتاح مساحة العمل" والمفتاح الأساسي لمساحة العمل. يحتاج معالج الإعداد إلى هذه المعلومات لتكوين الوكيل بشكل صحيح وضمان أنه يمكنه التواصل مع Azure Monitor.

1. [دفع البيانات التشخيصية إلى مساحة العمل.](https://go.microsoft.com/fwlink/?linkid=2128284) يمكنك نقل بيانات التشخيص من مستأجر WVD إلى Log Analytics لمساحة العمل.

1. [تحديد المشاكل](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) الداخلية أو الخارجية المتعلقة ب WVD وتشخصها.

لمعرفة المزيد حول تكوين أداة تشخيص الخدمة ل WVD، راجع استخدام تحليلات السجل لم الميزة التشخيصية.