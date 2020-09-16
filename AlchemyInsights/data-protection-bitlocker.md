---
title: داتابروتيكتيون-Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731226"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>تمكين تشفير Bitlocker باستخدام Intune

 يمكن استخدام نهج حماية نقطه نهاية Intune لتكوين إعدادات تشفير Bitlocker لأجهزه Windows. لمزيد من المعلومات ، راجع [إعدادات Windows 10 (والإصدارات الأحدث) لحماية الاجهزه باستخدام Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
يجب ان تكون علي علم بان العديد من الاجهزه الجديدة التي تقوم بتشغيل Windows 10 تدعم تشفير Bitlocker التلقائي ، الذي يتم تشغيله بدون تطبيق نهج MDM. قد يؤثر هذا علي تطبيق النهج في حال تم تكوين الإعدادات غير الافتراضية. راجع الاسئله المتداولة التالية لمزيد من التفاصيل.
 
للحصول علي معلومات حول استكشاف أخطاء bitlocker وإصلاحها ، راجع [استكشاف أخطاء نهج bitlocker وإصلاحها في Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**الأسئلة المتداولة**

 س: ما هي إصدارات تشفير أجهزه دعم Windows التي تستخدم نهج حماية نقطه النهاية ؟<br>
 ج: يتم تطبيق الإعدادات الموجودة في نهج حماية نقطه نهاية Intune باستخدام [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). لا تدعم كل إصدارات Windows أو إصداراتها التي تعتمد Bitlocker CSP. <br><br>
      في الوقت الحالي ، يتم دعم إصدارات Windows التالية: Enterprise و التعليم والهاتف المحمول والمؤسسة المحمولة والاحترافية (الإصدار 1809 والإصدارات الأحدث).
 
س: إذا تم تشفير جهاز بالفعل بواسطة Bitlocker باستخدام الإعدادات الافتراضية لنظام التشغيل التلقائي لأسلوب التشفير وقوه التشفير (128 إكستس) ، سيتم تطبيق نهج باستخدام إعدادات مختلفه تلقائيا بتشغيل الإعدادات الجديدة ؟<br>
ج: لا. لتطبيق إعدادات التشفير الجديدة ، يجب فك تشفير محرك الاقراص أولا.<br><br>
**ملاحظه:** بالنسبة إلى الاجهزه التي يتم تسجيلها باستخدام Autopilot ، لا يتم تشغيل التشفير التلقائي الذي سيحدث اثناء OOBE حتى يتم تقييم نهج Intune ، مما يسمح باستخدام الإعدادات المستندة إلى النهج في مكان الافتراضيات لنظام التشغيل.
 
س: إذا تم تشفير جهاز كنتيجة لتطبيق النهج Intune ، فهل سيتم فك تشفيره عند أزاله هذا النهج ؟<br>
ج: لا تؤدي أزاله النهج المرتبط بالتشفير إلى فك تشفير محركات الاقراص التي تم تكوينها.
 
س: لماذا يعرض نهج التوافق ل Intune عدم تمكين Bitlocker لجهازي ، علي الرغم من انه ؟<br>
ج: يستخدم الاعداد "تم تمكين Bitlocker" في نهج التوافق في Intune لعميل مصادقه الحماية الخاصة بجهاز Windows (دها). يقيس هذا العميل حاله الجهاز فقط في وقت التمهيد. إذا لم يتم أعاده تشغيل جهاز منذ اكتمال تشفير Bitlocker ، فلن تقوم خدمه عميل دها بالإبلاغ عن Bitlocker كما هو نشط.
 
 