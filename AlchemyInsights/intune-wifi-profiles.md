---
title: ملفات تعريف Wi-Fi Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: 5e5258806c8a38965467a8878bc8ac922c2668f21abe3602f479dcdaff8c9b5b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028207"
---
# <a name="intune-wi-fi-profiles"></a>ملفات تعريف Wi-Fi Intune

يعتمد نجاح Wi-Fi اتصال عملاء MDM على ملف تعريف تم نشره بشكل صحيح يعكس متطلبات بنية Wi-Fi الأساسية الخاصة بالشركة. لمراجعة الإعدادات المناسبة ل الأنظمة الأساسية للعميل التي تحقق منها، راجع: 

[إضافة Wi-Fi للأجهزة التي تعمل بنظام التشغيل Android في Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[أضف Wi-Fi لأجهزة Android Enterprise المخصصة والمدارة بالكامل في Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[أضف Wi-Fi الإعدادات الخاصة بأجهزة iOS وiPadOS في Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[إضافة Wi-Fi الإعدادات Windows 10 والأجهزة اللاحقة في Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[استيراد Wi-Fi جديدة للأجهزة Windows Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**المشاكل الشائعة**

**أقوم بنشر ملف تعريف Wi-Fi يعتمد على شهادة تم نشرها محددة في Wi-Fi التعريف. ومع ذلك، تظهر ملفات تعريف التكوين حالة خطأ.**

تحقق من استلام جهازك للشهادة.

1. في Intune، انتقل إلى **كافة الأجهزة** وحدد الجهاز > **تكوين الجهاز.**

2. تحقق من أن كل ملفات التعريف المتوقعة مدرجة وفي حالة ناجحة.

3. بالنسبة لملف تعريف Android، إذا كان لديك شهادات وسيطة في سلسلة الشهادات، فتأكد من نشرها على أجهزة Android.

    للتحقق من حالة الشهادة، انتقل إلى **ملفات تعريف** تكوين الجهاز  >    >  **شهادة خصائص CA وسيطة** ل Android  >    >  .

إذا استمرت الأخطاء في رؤية الأخطاء، فراجع الإجراءات وأقسام استكشاف الأخطاء وإصلاحها. لمزيد من المعلومات، راجع نظرة عامة حول استكشاف الأخطاء وإصلاحها لملفات تعريف شهادات [SCEP باستخدام Microsoft Intune.](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

**لقد نشرت ملف تعريف Wi-Fi على جهاز. يظهر Intune نجاحه، ولكن الجهاز لا يتصل بشبكة Wi-Fi.**

تعني الحالة الناجحة أن Intune قد نشر ملف التعريف بنجاح كما تم تكوينه. ومع ذلك، قد لا تتطابق هذه التكوينات مع متطلبات الشبكة و/أو المصادقة. للحصول على مزيد من التفاصيل حول الاتصال الذي تم محاولة الاتصال به، راجع السجلات في خدمة المصادقة والبنية الأساسية (على وحدة التحكم Wi-Fi نقطة الوصول وخادم NPS/نصف القطر). قد تحتاج إلى العمل مع فريق البنية الأساسية للشبكة، أو مورد Wi-Fi جهة خارجية، لجمع السجلات ومراجعتها.