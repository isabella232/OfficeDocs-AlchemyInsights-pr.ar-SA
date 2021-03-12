---
title: مراقبة الوصول المشروط
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708661"
---
# <a name="monitoring-conditional-access-for-exchange"></a>مراقبة الوصول الشرطي ل Exchange

سيتلقى المستخدمون المستهدفون الذين لديهم وصول مشروط رسالة بريد إلكتروني إعلام إذا لم يلبيوا متطلبات الوصول إلى مؤسستك. لحل هذه المشكلة، نوصي باستخدام حل واحد أو أكثر من الحلول التالية:

- إذا كان من المفترض أن يتم تسجيل الجهاز، فنصح المستخدمين بأن يرحلوا إلى تطبيق Company Portal وتحقق من ظهوره في Company Portal. وإذا لم يحدث ذلك، يجب على المستخدم تسجيل الجهاز.
- في مدخل Azure، انتقل إلى Intune > توافق الجهاز. ضمن "جهاز العرض"، انقر فوق توافق الجهاز. اشاهد تقرير توافق الجهاز للتحقق من وضع علامة على جهاز المستخدم كمتوافق.
- في مدخل Azure، انتقل إلى Intune > توافق الجهاز. ضمن "إدارة"، انقر فوق "سياسات". في قائمة سياسات التوافق، تحقق من تعيين ملف تعريف إلى جهاز المستخدم. إذا لم يتم تعيين ملف تعريف، لن يتمكن Intune من تأكيد حالة توافق الجهاز.
- تحرير تعيين الوصول المشروط للمستخدم.

1. في مدخل Azure، انتقل إلى "سياسات الوصول المشروط إلى **Intune".**  >    >  
2. حدد نهج من القائمة.
3. انقر فوق المستخدمين والمجموعات.
4. لاستهداف نهج معين لأحد الأشخاص، أضفه إلى القائمة "تضمين". للتأكد من حذف شخص من النهج، أضفه إلى القائمة "استبعاد".

ارتباطات مفيدة:

[نظرة عامة حول توافق الجهاز](https://docs.microsoft.com/intune/device-compliance-get-started)

[استكشاف الأخطاء الم CA وإصلاحها](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[نهج استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[مراقبة توافق أجهزة Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

ملاحظة: هذه الخطوات مفيدة فقط في استكشاف الأخطاء في ميزة الوصول المشروط ل Azure Active Directory وإصلاحها. من الممكن أيضا فحص جهاز يمنع الوصول إلى البريد الإلكتروني الخاص به باستخدام نهج Exchange. يمكن العثور على مزيد من المعلومات حول إدارة أجهزة Exchange [هنا]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
