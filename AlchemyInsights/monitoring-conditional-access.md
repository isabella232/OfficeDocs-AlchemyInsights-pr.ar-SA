---
title: مراقبه الوصول الشرطي
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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366415"
---
# <a name="monitoring-conditional-access-for-exchange"></a>مراقبه الوصول الشرطي ل Exchange

سيتلقى المستخدمون الذين يستهدفون access الشرطي بريدا الكترونيا للاعلام إذا لم يستوفوا متطلبات الوصول الخاصة بمؤسسك. لحل هذه المشكلة ، نوصي باجراء واحد أو أكثر من الحلول التالية:

- إذا كان الجهاز بريسوميد بالتسجيل ، فيمكنك اشعار المستخدم بالانتقال إلى تطبيق مدخل الشركة والتحقق من انه يظهر في مدخل الشركة. إذا لم يكن كذلك ، فيجب علي المستخدم تسجيل الجهاز.
- في مدخل Azure ، انتقل إلى التوافق مع جهاز Intune >. ضمن جهاز العرض ، انقر فوق توافق الجهاز. اعرض تقرير توافق الاجهزه للتحقق من انه تم وضع علامة علي جهاز المستخدم علي انه متوافق.
- في مدخل Azure ، انتقل إلى التوافق مع جهاز Intune >. ضمن أداره ، انقر فوق النهج. في قائمه نهج التوافق ، تحقق من انه تم تعيين ملف تعريف لجهاز المستخدم الخاص بك. إذا لم يتم تعيين اي ملف تعريف ، فلن يتمكن Intune من التحقق من حاله توافق الجهاز.
- تحرير تعيين الوصول الشرطي الخاص بالمستخدم.

1. في مدخل Azure ، انتقل إلى **Intune**  >  **نهج الوصول المشروط**ل Intune  >  **Policies**.
2. حدد نهجا من القائمة.
3. انقر فوق المستخدمون والمجموعات.
4. لاستهداف نهج معين في شخص ما ، أضفه إلى قائمه التضمين. للتاكد من حذف شخص من النهج ، أضفه إلى قائمه الاستبعاد.

الارتباطات المفيدة:

[نظره عامه علي توافق الاجهزه](https://docs.microsoft.com/intune/device-compliance-get-started)

[استكشاف أخطاء المراجع المصدقة](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[نهج استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[مراقبه توافق جهاز Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

ملاحظه: هذه الخطوات مفيده فقط في استكشاف الأخطاء وإصلاحها في الوصول الشرطي لميزه Azure Active Directory. من الممكن أيضا اجراء فحص للجهاز حظر الوصول إلى البريد الكتروني باستخدام نهج Exchange. يمكن العثور علي مزيد من المعلومات حول أداره أجهزه Exchange [هنا](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).
