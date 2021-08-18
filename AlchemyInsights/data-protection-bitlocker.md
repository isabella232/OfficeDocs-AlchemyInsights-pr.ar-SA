---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118557"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>تمكين تشفير Bitlocker باستخدام Intune

يمكن استخدام Endpoint Protection Intune لتكوين إعدادات تشفير Bitlocker Windows الأجهزة. لمزيد من المعلومات، [راجع Windows 10 (واللاحقة) لحماية الأجهزة باستخدام Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

بالإضافة إلى نهج Endpoint Protection يوجد أيضا تقرير تشفير يوفر طريقة عرض أكثر تفصيلا حول حالة التشفير للأجهزة. يمكن الوصول إلى هذا التقرير من مدخل MEM ضمن الأجهزة > **جهاز العرض**، ثم ضمن تكوين **حدد** [تقرير التشفير](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

إذا لم يتم تمكين Bitlocker كما هو متوقع أو إذا كان ملف التعريف المستخدم لتمكين Bitlocker في حالة خطأ، فيرجى مراجعة تقرير التشفير للحصول على فهم أفضل لل سبب حدوث السلوك.

للعثور على تفاصيل حول كيفية تفسير التقرير بما في ذلك قيم حالة التشفير المختلفة، راجع مراقبة تشفير الأجهزة [باستخدام Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

يجب أن تكون على علم بأن العديد من الأجهزة Windows 10 تدعم تشفير Bitlocker التلقائي، الذي يتم تشغيله بدون تطبيق نهج MDM. قد يؤثر ذلك على تطبيق النهج إذا تم تكوين إعدادات غير افتراضية. راجع الأسئلة الشائعة التالية للحصول على مزيد من التفاصيل.

للحصول على معلومات حول استكشاف مشاكل bitlocker وإصلاحها، راجع استكشاف مشاكل سياسات [BitLocker](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)وإصلاحها في Microsoft Intune .
 
 
**الأسئلة المتداولة**

س: ما هي إصدارات Windows تشفير أجهزة الدعم باستخدام Endpoint Protection؟<br>
ج: يتم تنفيذ الإعدادات في Intune Endpoint Protection باستخدام [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). لا تدعم كل إصدارات أو إصدارات Windows Bitlocker CSP. <br><br>

س: كيف يمكن تمكين Bitlocker على الأجهزة دون الحاجة إلى تفاعل المستخدم النهائي؟<br>
ج: طالما تم تحقيق المتطلبات الأساسية الضرورية، فمن الممكن تمكين Bitlocker "التشفير الصامت" من خلال Intune. راجع تفاصيل متطلبات الجهاز وإعدادات النهج على سبيل المثال لتمكين التشفير الصامت في المستعرض التالي: تمكين تشفير [Bitlocker بصمت](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

س: إذا كان الجهاز مشفرا بالفعل باستخدام Bitlocker باستخدام إعدادات نظام التشغيل الافتراضية لطريقة التشفير وقوة التشفير (XTS-AES-128)، فهل سيتم تطبيق نهج بإعدادات مختلفة تلقائيا على إعادة تشفير محرك الأقراص باستخدام الإعدادات الجديدة؟<br>
ج: لا. لتطبيق إعدادات التشفير الجديدة، يجب أولا فك تشفير محرك الأقراص.<br><br>
**ملاحظة:** بالنسبة للأجهزة التي يتم تسجيلها باستخدام Autopilot، لا يتم تشغيل التشفير التلقائي الذي سيحدث أثناء OOBE حتى يتم تقييم نهج Intune، مما يسمح باستخدام الإعدادات المستندة إلى النهج في مكان الإعدادات الافتراضية ل OS.
 
س: إذا تم تشفير جهاز نتيجة لتطبيق نهج Intune، فهل سيتم فك تشفيره عند إزالة هذا النهج؟<br>
أ: لا تؤدي إزالة النهج المرتبط بالتشفير إلى فك تشفير محركات الأقراص التي تم تكوينها.
 
س: لماذا يظهر نهج التوافق في Intune أن جهازي لا يقوم بتمكين Bitlocker، على الرغم من أنه تم تمكينه؟<br>
ج: يستخدم الإعداد "تمكين Bitlocker" في نهج التوافق في Intune عميل Windows حالة الجهاز (DHA). يقيس هذا العميل حالة الجهاز فقط في وقت التشغيل. وبالتالي، إذا لم يتم إعادة تشغيل الجهاز منذ اكتمال تشفير Bitlocker، لن تقوم خدمة عميل DHA ب الإبلاغ عن Bitlocker على أنه نشط.
 
 