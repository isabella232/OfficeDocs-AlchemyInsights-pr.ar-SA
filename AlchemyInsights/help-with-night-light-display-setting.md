---
title: تعليمات حول إعداد عرض الضوء الليلي
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404137"
---
# <a name="help-with-the-night-light-display-setting"></a>تعليمات حول إعداد عرض الضوء الليلي

لمعرفة المزيد حول إعدادات عرض الوقت الليلي، راجع تعيين العرض [للوقت الليلي في Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).

إذا كانت خيارات الضوء الليلي باللون الرمادي في الإعدادات، فتحقق من برنامج تشغيل العرض: 

1. انقر فوق مربع البحث على شريط المهام وا اكتب **إدارة الأجهزة**، ثم حدد **إدارة الأجهزة** في نتائج البحث.
1. توسيع **محولات العرض**. 

لسوء الحظ، لا تتوفر ميزة الضوء الليلي إذا كان جهازك يستخدم برنامج تشغيل DisplayLink أو برنامج تشغيل عرض أساسي.

تستخدم ميزة الضوء الليلي تقنية الرسومات الحديثة، لذلك قد تحتاج إلى تحديث برنامج تشغيل العرض:  

- تحقق من وجود تحديثات عن طريق الذهاب إلى **بدء** تحديث الإعدادات  >    >  **&**  >  **Windows Update** الأمان التحقق من وجود  >  **تحديثات**.  

OR

- تفضل بزيارة موقع ويب دعم الشركة المصنعة للأجهزة لتنزيل أحدث برامج تشغيل العرض وتثبيتها يدويا.

## <a name="reset-night-light-in-the-registry"></a>إعادة تعيين الضوء الليلي في السجل

إذا لم ينجح تحديث برنامج تشغيل جهاز العرض، فقد تحتاج إلى إعادة تعيين الضوء الليلي في السجل.  

**تنبيه:** يوصى بإجراء خطوة استكشاف الأخطاء وإصلاحها هذه للمستخدمين المتقدمين فقط. قد تحدث مشاكل خطيرة إذا قمت بتعديل السجل بشكل غير صحيح. لمزيد من الحماية، قم ب إنشاء سجل قبل تعديله حتى تتمكن من استعادته في حالة حدوث مشاكل.

1. في مربع البحث، اكتب **regedit**، ثم حدد **محرر السجل** في نتائج البحث.

1. انتقل إلى مفتاح التسجيل التالي: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. تصدير المفتاح الفرعي التالي ثم حذفه:$$windows.data.bluelightreduction.bluelightreductionstate

1. تصدير المفتاح الفرعي التالي ثم حذفه:$$windows.data.bluelightreduction.settings

1. أعد تشغيل Windows وتحقق مما إذا كانت خيارات الضوء الليلي متوفرة.


