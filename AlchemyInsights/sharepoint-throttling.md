---
title: SharePoint على الانترنت اختناق
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931429"
---
# <a name="sharepoint-online-throttling"></a>SharePoint على الانترنت اختناق

**هام:** يعمل العديد من عملاء SharePoint Online و OneDrive على تشغيل تطبيقات مهمة للأعمال مقابل الخدمة التي تعمل في الخلفية. وتشمل هذه ترحيل المحتوى، منع فقدان البيانات (DLP)، وحلول النسخ الاحتياطي. خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية وموثوقة للمستخدمين الذين يعتمدون على الخدمة أكثر من أي وقت مضى في سيناريوهات العمل عن بعد.

ولدعم هذا الهدف، قمنا بتنفيذ قيود خنق أكثر صرامة على تطبيقات الخلفية (الترحيل وDLP وحلول النسخ الاحتياطي) خلال ساعات النهار في أيام الأسبوع. يجب أن تتوقع أن تحقق هذه التطبيقات إنتاجية محدودة جدًا خلال هذه الأوقات. ومع ذلك ، خلال ساعات المساء وعطلة نهاية الأسبوع للمنطقة ، ستكون الخدمة جاهزة لمعالجة حجم أكبر بكثير من الطلبات من تطبيقات الخلفية.

**SharePoint على الانترنت اختناق**

يستخدم SharePoint Online الاختناق للحفاظ على الأداء الأمثل وموثوقية خدمة SharePoint Online. الاختناق يحد من عدد إجراءات المستخدم أو المكالمات المتزامنة (بواسطة البرنامج النصي أو التعليمات البرمجية) لمنع الإفراط في استخدام الموارد. لمزيد من المعلومات، يرجى زيارة الروابط أدناه.

- [تجنب الحصول على خنق أو حظر في SharePoint عبر الإنترنت](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [ترحيل البيانات واختناق SPO](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [SharePoint عبر الإنترنت وOneDrive سرعة الترحيل](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [التعامل مع اختناق SharePoint Online باستخدام التراجع الأسي](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [تخطيط القدرات واختبار التحميل SharePoint Online](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

