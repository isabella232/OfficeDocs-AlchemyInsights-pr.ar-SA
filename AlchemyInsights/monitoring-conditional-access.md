---
title: مراقبة الوصول الشرطي
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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975088"
---
# <a name="monitoring-conditional-access-for-exchange"></a>مراقبة الوصول الشرطي Exchange

سيتلقى المستخدمون المستهدفون الذين لديهم حق وصول شرطي رسالة بريد إلكتروني إعلام إذا لم يلبيوا متطلبات الوصول الخاصة بالم مؤسستك. لحل هذه المشكلة، نوصي بحل واحد أو أكثر من الحلول التالية:

- إذا كان من المفترض أن يكون الجهاز مسجلا، فنصح المستخدم الانتقال إلى تطبيق Company Portal وتحقق من ظهوره في Company Portal. وإذا لم يحدث ذلك، يجب على المستخدم تسجيل الجهاز.
- في مدخل Azure، انتقل إلى Intune > توافق الجهاز. ضمن جهاز العرض، انقر فوق توافق الجهاز. اشاهد تقرير توافق جهازك للتحقق من وضع علامة على جهاز المستخدم كمتوافق.
- في مدخل Azure، انتقل إلى Intune > توافق الجهاز. ضمن إدارة، انقر فوق سياسات. في قائمة سياسات التوافق، تحقق من تعيين ملف تعريف إلى جهاز المستخدم. إذا لم يتم تعيين ملف تعريف، لن يتمكن Intune من تأكيد حالة توافق الجهاز.
- تحرير تعيين الوصول الشرطي للمستخدم.

1. في مدخل Azure، انتقل إلى **Intune**  >  **Conditional access**  >  **Policies**.
2. حدد نهج من القائمة.
3. انقر فوق المستخدمون والمجموعات.
4. لاستهداف نهج معين لشخص ما، قم بإضافته إلى القائمة تضمين. للتأكد من حذف شخص من النهج، أضفه إلى القائمة استبعاد.

ارتباطات مفيدة:

[نظرة عامة حول توافق الجهاز](https://docs.microsoft.com/intune/device-compliance-get-started)

[استكشاف الأخطاء الم CA وإصلاحها](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[نهج استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[مراقبة توافق أجهزة Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

ملاحظة: هذه الخطوات مفيدة فقط في استكشاف الأخطاء وإصلاحها لمميزة Azure Active Directory الوصول الشرطي. من الممكن أيضا فحص جهاز يمنع الوصول إلى البريد الإلكتروني باستخدام Exchange المستخدم. يمكن العثور على مزيد Exchange حول إدارة الأجهزة [هنا]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
