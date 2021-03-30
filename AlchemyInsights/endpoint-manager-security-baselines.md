---
title: EndPoint Manager - خطوط الأمان الأساسية
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420691"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager - خطوط الأمان الأساسية

إن خطوط الأمان الأساسية هي مجموعات مكونة مسبقا من إعدادات Windows تساعدك على تطبيق إعدادات الأمان الموصى بها من قبل فرق الأمان ذات الصلة. يمكن تخصيص هذه الأساسات لتقديم الإعدادات والقيم المطلوبة فقط. لمزيد من المعلومات حول خطوط الأمان الأساسية، راجع استخدام خطوط الأمان الأساسية لتكوين أجهزة [Windows 10 في Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

توجد حاليا خطوط أساسية لهذه المنتجات:

- إعدادات أمان Windows MDM
- Microsoft Defender for EndPoint Security
- Microsoft Edge

يتم تحديث كل أساس بشكل دوري، كما يتم إصداره في إصدارات تزايدية. يضيف كل إصدار الإعدادات أو يزيلها من الإصدار السابق للتأكد من أن الأساس يلبي الإرشادات الحالية. تسمح وحدة تحكم خطوط الأمان الأساسية في أمان نقطة النهاية بمقارنة إصدارات مختلفة عن طريق جعل التغييرات من إصدار إلى إصدار مرئية.

للحصول على إرشادات حول كيفية تغيير إصدار الأساس الذي يتم نشره بفعالية أكبر، راجع إدارة ملفات تعريف خط الأمان الأساسي [في Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

بعد نشر أساس أمان، يمكنك مراقبة حالة النشر ومراجعة الإعدادات على أساس كل جهاز على حدة.

**ملاحظة:** قد تستغرق بيانات إعداد التقارير لخط الأساسات ما يصل إلى 24 ساعة لكي تظهر من النشر الأولي إلى جهاز، وما يصل إلى 6 ساعات لمزيد من التحديثات. 

السبب الأكثر شيوعا لعدم تطبيق إعداد الأساس هو أن نفس الإعداد يتم استخدامه في ملف تعريف مختلف. يمكن التحقق من هذا السيناريو لجهاز معين عن طريق تحديد هذا الجهاز من ضمن عقدة حالة الجهاز لملف تعريف أساسي الأمان. للحصول على التفاصيل، راجع [حل التعارضات الخاصة باساسيات الأمان](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).