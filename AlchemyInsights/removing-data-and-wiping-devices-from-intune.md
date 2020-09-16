---
title: أزاله البيانات والاجهزه الويبينجه من Intune
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
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701270"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>أزاله البيانات والاجهزه الويبينجه من Intune

يمكن استخدام الإجراءات البعيدة للغاء الجهاز ومسح الجهاز لأزاله بيانات الشركة المدارة بواسطة Intune أو لاجراء أعاده تعيين المصنع وإرجاع الجهاز إلى إعداداته الافتراضية.

1. سجل دخولك إلى أداره أجهزه Microsoft 365 ، وانتقل إلى **الاجهزه**  >  **كل الاجهزه**.
2. حدد الجهاز الذي تريد مسحه.
3. حدد نوع المسح البعيد الذي تريد القيام به. قم بإيقاف حذف المعلومات التنظيمية فقط ، في حين مناديل الجهاز بالبالكامل إلى إعدادات المصنع.
4. حدد **نعم** للتاكيد. حتى ينتهي المسح ، تظهر حاله اجراء الجهاز بالشكل المعلق.</br>
    بعد اكتمال الاجراء ، لن تتمكن من رؤية الجهاز المحمول في قائمه الاجهزه المدارة.

**ملاحظه** لا يمكن أزاله بيانات الشركة من الاجهزه المنضمة إلى Azure AD.

للحصول علي التفاصيل الكاملة لتاثير الإيقاف والمسح ، بما في ذلك ما يتم الاحتفاظ به وحذفه ، راجع [أزاله الاجهزه باستخدام مسح أو إيقاف أو إلغاء الجهاز](https://docs.microsoft.com/intune/devices-wipe).

لمسح كل البيانات من جهاز macOS ، راجع [محو كل البيانات من جهاز macOS](https://docs.microsoft.com/intune/device-erase).