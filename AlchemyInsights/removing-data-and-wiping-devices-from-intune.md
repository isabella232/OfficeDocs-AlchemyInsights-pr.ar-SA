---
title: إزالة البيانات ومسح الأجهزة من Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438791"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>إزالة البيانات ومسح الأجهزة من Intune

يمكن استخدام إجراءات الجهاز "تقاعد" و"مسح الجهاز" عن بعد لإزالة بيانات الشركة التي تديرها Intune أو لإجراء إعادة تعيين المصنع وإعادة الجهاز إلى إعداداته الافتراضية.

1. تسجيل الدخول إلى Microsoft 365 إدارة الأجهزة، ثم انتقل إلى **الأجهزة**  >  **كافة الأجهزة**.
2. حدد الجهاز الذي تريد مسحه.
3. حدد نوع المسح عن بعد الذي تريد القيام به. يحذف التقاعد المعلومات التنظيمية فقط، بينما يقوم المسح الكامل باستعادة الجهاز إلى إعدادات المصنع.
4. حدد **نعم** للتأكيد. حتى انتهاء المسح، تظهر حالة إجراء الجهاز كـ "معلّل معلق".</br>
    بعد اكتمال الإجراء، لن ترى الجهاز المحمول في قائمة الجهاز المُدار.

**ملاحظة** لا يمكن إزالة بيانات الشركة من الأجهزة التي تم الانضمام إليها إلى Azure AD.

للحصول على التفاصيل الكاملة لتأثير إجراءات التقاعد والمسح، بما في ذلك ما يتم الاحتفاظ به وما يتم حذفه، راجع [إزالة الأجهزة باستخدام المسح أو التقاعد أو إلغاء تشغيل الجهاز يدويًا](https://docs.microsoft.com/intune/devices-wipe).

لمسح كافة البيانات من جهاز macOS، راجع [محو كافة البيانات من جهاز macOS](https://docs.microsoft.com/intune/device-erase).