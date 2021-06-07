---
title: مشاكل الأداء ل Microsoft Defender ل Endpoint على Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793544"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>مشاكل الأداء ل Microsoft Defender ل Endpoint على Linux

ترشدك هذه المقالة عبر خطوات تحديد مشاكل الأداء ل Microsoft Defender ل Endpoint على Linux.

من المهم التحقق أولا من حل المشكلة التي تواجهها باستخدام [الإصدار الأخير.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

لبدء التحقيق، راجع استكشاف مشاكل الأداء وإصلاحها ل [Microsoft Defender ل Endpoint على Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).

## <a name="exclusions"></a>الاستثناءات

يمكن أن تساعد الاستثناءات على الحد من مشاكل الأداء. راجع استثناءاتك قبل البدء بحيث تكون أي مخاطر إضافية معروفة وموثقة.

لمزيد من المعلومات، راجع تكوين الاستثناءات ل Microsoft Defender ل Endpoint على Linux والتحقق من [صحتها.](/microsoft-365/security/defender-endpoint/linux-exclusions)

عندما يكون لديك ملفات متعددة & مجلدات يجب استبعادها وكلها على نقطة التركيب نفسها، قد يكون من الأسهل استبعاد نقطة التركيب. بدءا من إصدار فبراير 101.22.80، يمكنك استبعاد نقطة تحميل كاملة.

على سبيل المثال، إذا كان /mnt/backup هو نقطة تحميل، يمكنك إضافة /mnt/backup إلى القائمة استبعاد عن طريق تشغيل هذا الأمر:

`$ mdatp exclusion folder add –path /mnt/backup`

**ملاحظة:** تؤدي إضافة استثناءات إلى زيادة خطر عدم الكشف عن البرامج الضارة ويجب معالجتها وتنفيذها بحرص.

## <a name="need-help"></a>هل تحتاج إلى مساعدة؟

لمساعدتك بالطريقة الأكثر فعالية، يمكنك تجميع البيانات التشخيصية قبل فتح حالة دعم.
