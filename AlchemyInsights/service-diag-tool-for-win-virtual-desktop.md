---
title: أداة تشخيص الخدمة لسطح المكتب Windows الظاهري
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052373"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>أداة تشخيص الخدمة لسطح المكتب Windows الظاهري

Windows يوفر سطح المكتب الظاهري (WVD) أداة تشخيص تسمح للمسؤولين بتحديد الأخطاء من خلال واجهة واحدة. تقوم هذه الأداة بتسجيل المعلومات ذات الصلة بالت تشخيص كلما تم استخدام WVD من قبل شخص تم تعيين دور WVD له. يحتوي كل سجل على معلومات حول دور WVD الذي يتضمنه النشاط، ورسائل الخطأ التي تظهر أثناء جلسة العمل، ومعلومات حول المستأجر والمستخدم. يمكن تكوين Azure Log Analytics لتسجيل سجل النشاط الذي أنشأته أداة التشخيص. إليك كيفية تنفيذ ذلك:

1. إنشاء مساحة عمل Log Analytics باستخدام [مدخل Azure](https://go.microsoft.com/fwlink/?linkid=2129500) أو [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [الاتصال Windows الكمبيوتر إلى Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). احصل على "مفتاح مساحة العمل" والمفتاح الأساسي لمساحة العمل. يحتاج معالج الإعداد إلى هذه المعلومات لتكوين الوكيل بشكل صحيح وضمان أنه يمكنه التواصل مع Azure Monitor.
1. [دفع البيانات التشخيصية إلى مساحة العمل.](https://go.microsoft.com/fwlink/?linkid=2128284) يمكنك نقل بيانات التشخيص من مستأجر WVD إلى Log Analytics لمساحة العمل.
1. [تحديد المشاكل](https://go.microsoft.com/fwlink/?linkid=2128338) الداخلية أو الخارجية المتعلقة ب WVD وتشخصها.

لمعرفة المزيد حول تكوين أداة تشخيص الخدمة ل WVD، راجع استخدام تحليلات السجل [لم الميزة التشخيصية](https://go.microsoft.com/fwlink/?linkid=2128084).
