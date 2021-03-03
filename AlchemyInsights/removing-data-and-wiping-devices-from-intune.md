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
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416300"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>إزالة البيانات ومسح الأجهزة من Intune

يمكن استخدام الإجراءين "إيقاف الجهاز" و"مسح الجهاز" عن بعد لإزالة بيانات الشركة المدارة بواسطة Intune أو لتنفيذ عملية إعادة ضبط المصنع وإعادة الجهاز إلى إعداداته الافتراضية.

1. سجل الدخول إلى Microsoft 365 Device Management، واذهب إلى **"الأجهزة**  >  **كافة الأجهزة".**
2. حدد الجهاز الذي تريد مسحه.
3. حدد نوع المسح عن بعد الذي تريد القيام به. يحذف إيقاف المعلومات التنظيمية فقط، بينما تستعيد عمليات المسح الكامل الجهاز إلى إعدادات المصنع الخاصة به.
4. حدد **"نعم"** لتأكيد الأمر. حتى تنتهي عملية المسح، تظهر حالة الإجراء "الجهاز" ك *"معلق للتقاعد".*
    بعد اكتمال الإجراء، لن ترى الجهاز المحمول بعد الآن في قائمة الجهاز المدار.

> [!NOTE]
> لا يمكن إزالة بيانات الشركة من الأجهزة المنضمة إلى Azure AD. 

للحصول على التفاصيل الكاملة حول تأثير إجراءات "إيقاف" و"مسح"، بما في ذلك ما تم الاحتفاظ به وما تم حذفه، راجع الوثائق التالية:

- [قم بإزالة الأجهزة باستخدام مسح](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)الجهاز أو إيقافه أو إلغاءه يدويا.
- [كيفية مسح بيانات الشركة فقط من تطبيقات Intune المدارة](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [مسح كل البيانات من جهاز macOS.](https://docs.microsoft.com/mem/intune/remote-actions/device-erase)