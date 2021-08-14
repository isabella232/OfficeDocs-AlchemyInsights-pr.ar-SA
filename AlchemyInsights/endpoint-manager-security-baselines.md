---
title: إدارة نقاط النهاية - أساسات الأمان
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
- "10064"
- "9003771"
ms.openlocfilehash: c13bc161b19a5fef1352beb28bdcc20110111a9a61a47433d82e1e69aff7f88d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978148"
---
# <a name="endpoint-manager---security-baselines"></a>إدارة نقاط النهاية - أساسات الأمان

أساسات الأمان هي مجموعات من إعدادات Windows مكوّنة مسبقاً تساعدك على تطبيق إعدادات الأمان التي يوصي بها فرق الأمان ذات الصلة. يمكن تخصيص هذه الأساسات لتقديم الإعدادات والقيم المرادة فقط. للحصول على مزيد من المعلومات حول أساسات الأمان، اطلع على [استخدام أساسات الأمان لتكوين أجهزة Windows 10 في Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

متوفر حالياً أساسات لهذه البرامج:

- إعدادات أمان Windows MDM
- أمان Microsoft Defender لنقطة النهاية
- Microsoft Edge

يُحدث كل أساس بشكل دوري ويطرح في الإصدارات المتزايدة. يضيف كل إصدار إعدادات من الإصدار السابق أو يزيلها لضمان استيفاء الأساس الإرشادات الحالية. تسمح وحدة التحكم في أساسات الأمان في أمان نقطة النهاية بالمقارنة بين الإصدارات المختلفة بإظهار التغييرات من إصدار إلى آخر.

للحصول على إرشادات حول كيفية تغيير إصدار الأساس الذي سيتم نشره بأعلى فاعلية، اطلع على [إدارة ملفات تعريف أساسات الأمان في Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

بعد نشر أحد أساسات الأمان، ستتمكّن من مراقبة حالة النشر ومراجعة الإعدادات على الأجهزة بشكل مستقل.

**ملاحظة:** قد يستغرق ظهور بيانات تقارير الأساسات من النشر الأولي إلى أحد الأجهزة ما يصل إلى 24 ساعة وقد يستغرق إجراء تحديثات إضافية ما يصل إلى 6 ساعات. 

يكّمن السبب الأكثر شيوعاً وراء عدم تطبيق أحد إعدادات الأساسات في أن الإعداد نفسه يُستخدم حالياً في ملف تعريف مختلف. يمكن التحقق من هذا السيناريو لجهاز معين من خلال تحديد هذا الجهاز من داخل عقدة "حالة الجهاز" لملف تعريف أساس الأمان. للحصول على التفاصيل، اطلع على [حل التعارضات بين أساسات الأمان](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).