---
title: ملفات تعريف Intune Wi-fi
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
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696248"
---
# <a name="intune-wi-fi-profiles"></a>ملفات تعريف Intune Wi-fi

يعتمد التنفيذ الناجح لاتصال Wi-fi لعملاء MDM علي ملف تعريف موزع بشكل صحيح يعكس متطلبات البنية الاساسيه للشركات Wi-fi. لمراجعه الإعدادات المناسبة للانظمه الاساسيه التي تقوم بالتحقق منها ، راجع: 

[أضافه إعدادات Wi-fi للاجهزه التي تعمل بنظام التشغيل Android في Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[أضافه إعدادات Wi-fi للاجهزه التي تعمل بنظام Android Enterprise المخصصة والاجهزه المدارة بالبالكامل في Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[أضافه إعدادات Wi-fi للاجهزه التي تعمل بنظام التشغيل iOS و إيبادوس في Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[أضافه إعدادات Wi-fi لنظام التشغيل Windows 10 والاجهزه الأحدث في Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[استيراد إعدادات Wi-fi لأجهزه Windows في Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**المشاكل الشائعة**

**أقوم بنشر ملف تعريف Wi-fi المعتمد علي شهادة منشوره محدده في ملف تعريف Wi-fi. ومع ذلك ، تعرض ملفات تعريف التكوين حاله خطا.**

تاكد من ان جهازك استلم الشهادة.

1. في Intune ، انتقل إلى **كل الاجهزه** وحدد **تكوين جهاز**> الجهاز.

2. تاكد من ان كل ملفات التعريف المتوقعة مدرجه وفي حاله ناجحه.

3. بالنسبة إلى ملف تعريف Android ، إذا كان لديك شهادات متوسطه في سلسله الشهادات ، فتاكد من نشرها علي أجهزه Android.

    للتحقق من حاله الشهادة ، انتقل إلى ملفات تعريف **تكوين الجهاز**الخاصة  >  **Profiles**  >  **Android intermediate CA**  >  **Properties**  >  **بالشهادات الموثوق بها**لنظام التشغيل Android وسيطه.

إذا استمر ظهور الأخطاء ، فراجع القسمين الإجراءات واستكشاف الأخطاء وإصلاحها. لمزيد من المعلومات ، راجع [نظره عامه حول استكشاف أخطاء ملفات تعريف شهادات سسيب وإصلاحها باستخدام Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**لقد قمت بنشر ملف تعريف Wi-fi إلى جهاز. يعرض Intune انه نجح ، ولكن الجهاز لا يتصل بشبكه Wi-fi.**

تعني الحالة ناجح ان يقوم Intune بنشر ملف التعريف كما تم تكوينه بنجاح. ومع ذلك ، قد لا تتطابق هذه التكوينات مع متطلبات الشبكة و/أو المصادقة. للحصول علي مزيد من التفاصيل حول الاتصال الذي تمت محاولته ، راجع السجلات في البنية الاساسيه وخدمه المصادقة (علي جهاز التحكم بنقطه وصول wi-fi وخادم NPS/Radius). قد يتعين عليك استخدام فريق البنية الاساسيه للشبكة ، أو مورد Wi-fi للجهة الخارجية ، لجمع السجلات ومراجعتها.