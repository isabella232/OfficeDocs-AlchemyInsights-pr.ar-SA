---
title: نصائح نهج DLP لا تعمل
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932573"
---
# <a name="dlp-policy-tip-issues"></a>مشكلات تلميح نهج DLP

**هام:** يعمل العديد من عملاء SharePoint Online و OneDrive على تشغيل تطبيقات مهمة للأعمال مقابل الخدمة التي تعمل في الخلفية. وتشمل هذه ترحيل المحتوى، منع فقدان البيانات (DLP)، وحلول النسخ الاحتياطي. خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية وموثوقة للمستخدمين الذين يعتمدون على الخدمة أكثر من أي وقت مضى في سيناريوهات العمل عن بعد.

ولدعم هذا الهدف، قمنا بتنفيذ قيود خنق أكثر صرامة على تطبيقات الخلفية (الترحيل وDLP وحلول النسخ الاحتياطي) خلال ساعات النهار في أيام الأسبوع. يجب أن تتوقع أن تحقق هذه التطبيقات إنتاجية محدودة جدًا خلال هذه الأوقات. ومع ذلك ، خلال ساعات المساء وعطلة نهاية الأسبوع للمنطقة ، ستكون الخدمة جاهزة لمعالجة حجم أكبر بكثير من الطلبات من تطبيقات الخلفية.

**نصائح سياسة DLP**

عند استخدام **نُهج DLP،** يمكن إعلام المستخدمين بانتهاك النهج باستخدام **نصائح النهج.** يمكن للمسؤولين تكوين تلميحات النهج لعرضأثناء اختبار نهج DLP أو عندما يكون النهج في وضع التطبيق الكامل.
  
لتكوين تلميحات النهج حول نهج DLP الخاص بك في مركز الأمان والامتثال في وضع التنفيذ الكامل، قم بما يلي:
  
- تأكد من **تمكين** تلميحات السياسة على قاعدة DLP باستخدام الخطوات [هنا](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

- تأكد من **تطابق المحتوى** الخاص بك مع ما هو **مطلوب** لتشغيل القاعدة الموضحة في هذه المقالة [هنا](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- يتم عرض تلميحات النهج في كل من OWA و Outlook. ومع ذلك، عند استخدام **Outlook 2013 أو أحدث،** يتم عرض تلميحات النهج فقط تحت ظروف معينة. يتم سرد هذه الشروط هنا: [الشروط المعتمدة لـ Outlook 2013 أو أحدث لعرض تلميحات النهج](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)

للحصول على معلومات إضافية حول نصائح سياسة DLP، راجع: [إظهار نصائح السياسة لسياسات DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  