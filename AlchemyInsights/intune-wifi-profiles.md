---
title: ملفات تعريف Wi-Fi Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554720"
---
# <a name="intune-wi-fi-profiles"></a>ملفات تعريف Wi-Fi Intune

يعتمد التنفيذ الناجح لاتصال Wi-Fi لعملاء MDM على ملف تعريف تم نشره بشكل صحيح يعكس متطلبات البنية الأساسية للواي فاي للشركات. لمراجعة الإعدادات المناسبة للأنظمة الأساسية العميلة التي تقوم بالتحقق منها، راجع: 

[إضافة إعدادات Wi-Fi للأجهزة التي تعمل بنظام التشغيل Android في Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[إضافة إعدادات Wi-Fi لأجهزة Android Enterprise المخصصة والمدارة بالكامل في Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[إضافة إعدادات Wi-Fi لأجهزة iOS وiPadOS في Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[إضافة إعدادات Wi-Fi لـ Windows 10 والأجهزة الأحدث في Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[استيراد إعدادات Wi-Fi لأجهزة Windows في Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**القضايا المشتركة**

**أقوم بنشر ملف تعريف Wi-Fi يعتمد على شهادة منشورة محددة في ملف تعريف Wi-Fi. ومع ذلك، تظهر ملفات تعريف التكوين حالة خطأ.**

تحقق من أن الجهاز قد تلقى الشهادة.

1. في Intune، انتقل إلى **كافة الأجهزة** وحدد الجهاز > **تكوين الجهاز**.

2. تحقق من أن كافة التشكيلات الجانبية المتوقعة مدرجة وفي حالة ناجحة.

3. بالنسبة لملف تعريف Android، إذا كان لديك شهادات متوسطة في سلسلة الشهادات، تأكد من نشرها على أجهزة Android.

    للتحقق من حالة الشهادة، انتقل إلى التشكيلات الجانبية لتكوين **الجهاز**  >  **Profiles**  >  **Android متوسطة CA**  >  **Properties**Certificate  >  **موثوق .**

إذا استمر عرض الأخطاء، راجع الإجراءات وأقسام استكشاف الأخطاء وإصلاحها. لمزيد من المعلومات، راجع [نظرة عامة لاستكشاف أخطاء ملفات تعريف شهادات SCEP مع Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**قمت بنشر ملف تعريف Wi-Fi على جهاز. Intune هو تبين أنه كان ناجحا، ولكن الجهاز لا يتصل واي فاي.**

حالة ناجحة يعني أن Intune نشر التشكيل الجانبي كما تم تكوينها بنجاح. ومع ذلك، قد لا تتطابق هذه التكوينات مع متطلبات الشبكة و/أو المصادقة. لمزيد من التفاصيل حول الاتصال الذي تمت محاولة الاتصال به، قم بمراجعة سجلات في البنية التحتية وخدمة المصادقة (على وحدة تحكم نقطة وصول Wi-Fi وخادم NPS/Radius). قد تحتاج إلى العمل مع فريق البنية الأساسية للشبكة، أو مع مورد Wi-Fi التابع لجهة خارجية، لجمع سجلات ومراجعةها.