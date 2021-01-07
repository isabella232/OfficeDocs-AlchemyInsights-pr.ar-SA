---
title: داتابروتيكشن-Bitlocker
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
ms.openlocfilehash: 482c08b31e4d97ca5cc9ec6e35e309cb7536036d
ms.sourcegitcommit: 58ac31a58c956a4d74f66bd4151a2311dc361b78
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/07/2021
ms.locfileid: "49778180"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>تمكين تشفير Bitlocker باستخدام Intune

يمكن استخدام نهج حماية نقطه نهاية Intune لتكوين إعدادات تشفير Bitlocker لأجهزه Windows. لمزيد من المعلومات ، راجع [إعدادات Windows 10 (والإصدارات الأحدث) لحماية الاجهزه باستخدام Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

بالاضافه إلى نهج حماية نقطه النهاية ، يوجد أيضا تقرير تشفير يوفر طريقه عرض أكثر تفصيلا لحاله التشفير للاجهزه. يمكن الوصول إلى هذا التقرير من مدخل ميم ضمن **ال> أجهزه التي تعرض جهاز العرض**، ثم ضمن **التكوين** تحديد [تقرير التشفير](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

إذا اكتشفت انه سيفشل تمكين Bitlocker بالشكل المتوقع أو إذا كان ملف التعريف الذي يتم استخدامه لتمكين Bitlocker في حاله خطا ، فالرجاء مراجعه تقرير التشفير للحصول علي فهم أفضل لسبب حدوث السلوك.

للبحث عن تفاصيل حول كيفيه تفسير التقرير بما في ذلك قيم حاله التشفير المختلفة ، راجع [تشفير جهاز المراقبة باستخدام Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

يجب ان تكون علي علم بان العديد من الاجهزه الجديدة التي تقوم بتشغيل Windows 10 تدعم تشفير Bitlocker التلقائي ، الذي يتم تشغيله بدون تطبيق نهج MDM. قد يؤثر هذا علي تطبيق النهج في حال تم تكوين الإعدادات غير الافتراضية. راجع الاسئله المتداولة التالية لمزيد من التفاصيل.

للحصول علي معلومات حول استكشاف أخطاء bitlocker وإصلاحها ، راجع [استكشاف أخطاء نهج bitlocker وإصلاحها في Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**الأسئلة المتداولة**

س: ما هي إصدارات تشفير أجهزه دعم Windows التي تستخدم نهج حماية نقطه النهاية ؟<br>
ج: يتم تطبيق الإعدادات الموجودة في نهج حماية نقطه نهاية Intune باستخدام [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). لا تدعم كل إصدارات Windows أو إصداراتها التي تعتمد Bitlocker CSP. <br><br>

س: كيف يمكن تمكين Bitlocker علي الاجهزه من دون الحاجة إلى تفاعل المستخدم النهائي ؟<br>
ج: طالما كانت المتطلبات الضرورية للإصدارات السابقة ممكنة لتمكين Bitlocker "التشفير التلقائي" عبر Intune. راجع تفاصيل متطلبات الجهاز وإعدادات النهج المثال لتمكين التشفير الصامت في المستند التالي: [يمكنك تمكين تشفير Bitlocker بدون مطالبه](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

س: إذا تم تشفير جهاز بالفعل بواسطة Bitlocker باستخدام الإعدادات الافتراضية لنظام التشغيل التلقائي لأسلوب التشفير وقوه التشفير (128 إكستس) ، سيتم تطبيق نهج باستخدام إعدادات مختلفه تلقائيا بتشغيل الإعدادات الجديدة ؟<br>
ج: لا. لتطبيق إعدادات التشفير الجديدة ، يجب فك تشفير محرك الاقراص أولا.<br><br>
**ملاحظه:** بالنسبة إلى الاجهزه التي يتم تسجيلها باستخدام Autopilot ، لا يتم تشغيل التشفير التلقائي الذي سيحدث اثناء OOBE حتى يتم تقييم نهج Intune ، مما يسمح باستخدام الإعدادات المستندة إلى النهج في مكان الافتراضيات لنظام التشغيل.
 
س: إذا تم تشفير جهاز كنتيجة لتطبيق النهج Intune ، فهل سيتم فك تشفيره عند أزاله هذا النهج ؟<br>
ج: لا تؤدي أزاله النهج المرتبط بالتشفير إلى فك تشفير محركات الاقراص التي تم تكوينها.
 
س: لماذا يعرض نهج التوافق ل Intune عدم تمكين Bitlocker لجهازي ، علي الرغم من انه ؟<br>
ج: يستخدم الاعداد "تم تمكين Bitlocker" في نهج التوافق في Intune لعميل مصادقه الحماية الخاصة بجهاز Windows (دا). يقيس هذا العميل حاله الجهاز فقط في وقت التمهيد. إذا لم يتم أعاده تشغيل جهاز منذ اكتمال تشفير Bitlocker ، فلن تقوم خدمه عميل دا بالإبلاغ عن Bitlocker كما هو نشط.
 
 