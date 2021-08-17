---
title: مشاكل تتعلق بإزالة جهاز تم إيقاف تشغيله أو إيقاف تشغيله من "مخزون الأجهزة"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 6eb59d16a1dab2de0e7a44faf9b34be6432342f9e20c94b6932e69e937751add
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891990"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>مشاكل تتعلق بإزالة جهاز تم إيقاف تشغيله أو إيقاف تشغيله من "مخزون الأجهزة"

لا يسمح Microsoft Defender ل Endpoint حاليا بإزالة سجل الجهاز يدويا لجهاز تم إيقاف تشغيله أو إيقاف تشغيله من "مخزون الجهاز".

لأغراض الأمان، يظل الجهاز في المدخل كسجل تاريخي لمدة تصل إلى 180 يوما. ومع ذلك، يتم إزالة بيانات الجهاز وفقا لفترة الاستبقاء التي تم تكوينها.

**ملاحظة:** يتم تبديل الجهاز غير المستخدم أو المفجوع  تلقائيا إلى حالة "غير نشط" بعد سبعة أيام. بالإضافة إلى ذلك، لا يتم حساب الأجهزة غير النشطة في آخر 30 يوما في البيانات التي تعكس درجة التعرض للضوء إدارة المخاطر والثغرات الأمنية أو Microsoft Secure Score للأجهزة.
 
إذا كنت لا تزال لا تريد رؤية أجهزة معينة في طريقة عرض "مخزون الجهاز"، فحاول وضع علامة جهاز لتصفية الجهاز الذي تم قطع تشغيله من طريقة عرض "مخزون الجهاز".

لمزيد من المعلومات، اطلع على:

[أجهزة إيقاف التشغيل من خدمة Microsoft Defender لنقطة النهاية](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[درجة التعرض للضوء في إدارة المخاطر والثغرات الأمنية](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[إصلاح أدوات الاستشعار غير الصحية في Microsoft Defender لنقطة النهاية](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[كيفية استخدام العلامات بفعالية (الجزء 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[كيفية استخدام العلامات بفعالية (الجزء 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[كيفية استخدام العلامات بفعالية (الجزء 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




