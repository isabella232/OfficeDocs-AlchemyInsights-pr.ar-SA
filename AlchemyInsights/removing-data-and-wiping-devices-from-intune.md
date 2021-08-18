---
title: إزالة البيانات ومسح الأجهزة من Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: 92673c4a2a0e0faa98d3ade5ca1f6aa687d4c94a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331028"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>إزالة البيانات ومسح الأجهزة من Intune

يمكن استخدام الإجراءين "إيقاف الجهاز" و"مسح الجهاز" عن بعد لإزالة بيانات الشركة المدارة بواسطة Intune أو لتنفيذ إعادة ضبط المصنع وإعادة الجهاز إلى إعداداته الافتراضية.

1. سجل دخولك Microsoft 365 إدارة الأجهزة، واذهب إلى **الأجهزة**  >  **كافة الأجهزة.**
2. حدد الجهاز الذي تريد مسحه.
3. حدد نوع المسح عن بعد الذي تريد القيام به. يحذف إيقاف تشغيل المعلومات التنظيمية فقط، في حين تستعيد عمليات المسح الكامل الجهاز إلى إعدادات المصنع الخاصة به.
4. حدد **نعم** لتأكيد الأمر. حتى تنتهي عملية المسح، تظهر حالة الإجراء الجهاز ك *إيقاف معلق*.
    بعد اكتمال الإجراء، لن ترى الجهاز المحمول في قائمة الجهاز المدار.

**ملاحظة:** لا يمكن إزالة بيانات الشركة من الأجهزة المنضمة إلى Azure AD. 

للحصول على التفاصيل الكاملة حول تأثير إجراءات "التقاعد والمسح"، بما في ذلك الإجراءات التي يتم الاحتفاظ بها والحذف، راجع الوثائق التالية:

- [قم بإزالة الأجهزة باستخدام مسح](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)الجهاز أو إيقافه أو إلغاء استخدامه يدويا.
- [كيفية مسح بيانات الشركة فقط من التطبيقات المدارة في Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [مسح كل البيانات من جهاز macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).