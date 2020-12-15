---
title: أداه تشخيص الخدمة لسطح مكتب Windows الظاهري
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
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/14/2020
ms.locfileid: "49676935"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>أداه تشخيص الخدمة لسطح مكتب Windows الظاهري

يوفر Windows Virtual Desktop (وفد) أداه تشخيص تتيح للمسؤولين تحديد الأخطاء عبر واجهه واحده. تسجل هذه الاداه معلومات ذات صله بالتشخيص عند استخدام وفد بواسطة شخص قام بتعيين دور وفد. يحتوي كل سجل علي معلومات حول دور وفد المضمن في النشاط ورسائل الخطا التي تظهر اثناء جلسة العمل والمعلومات المتعلقة بالمستاجر والمستخدم. يمكن تكوين تحليلات سجلات Azure للتقاط سجل النشاط الذي تم إنشاؤه بواسطة أداه التشخيص. إليك كيفية تنفيذ ذلك:

1. إنشاء مساحة عمل لتحليلات السجلات باستخدام [مدخل azure](https://go.microsoft.com/fwlink/?linkid=2129500) أو [azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [توصيل أجهزه كمبيوتر Windows ب Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). احصل علي معرف مساحة العمل والمفتاح الأساسي لمساحة العمل الخاصة بك. يحتاج معالج الاعداد إلى هذه المعلومات لتكوين العامل بشكل صحيح وللتاكد من انه يمكنه التواصل مع جهاز عرض Azure.
1. [دفع بيانات التشخيص إلى مساحة العمل](https://go.microsoft.com/fwlink/?linkid=2128284). يمكنك دفع بيانات التشخيص من مستاجر وفد الخاص بك إلى تحليلات السجل لمساحة العمل الخاصة بك.
1. [تحديد المشاكل](https://go.microsoft.com/fwlink/?linkid=2128338) الداخلية أو الخارجية وتشخيصها بالنسبة إلى وفد.

لمعرفه المزيد حول تكوين أداه تشخيص الخدمة ل وفد ، راجع [استخدام تحليلات السجلات لميزه التشخيص](https://go.microsoft.com/fwlink/?linkid=2128084).
