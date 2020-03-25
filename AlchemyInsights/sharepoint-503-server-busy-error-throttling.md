---
title: SharePoint اختناق عبر الإنترنت
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931213"
---
# <a name="sharepoint-online-throttling"></a>SharePoint اختناق عبر الإنترنت

**هام:** يعمل العديد من عملاء SharePoint Online و OneDrive على تشغيل تطبيقات مهمة للأعمال مقابل الخدمة التي تعمل في الخلفية. وتشمل هذه ترحيل المحتوى، منع فقدان البيانات (DLP)، وحلول النسخ الاحتياطي. خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية وموثوقة للمستخدمين الذين يعتمدون على الخدمة أكثر من أي وقت مضى في سيناريوهات العمل عن بعد.

ولدعم هذا الهدف، قمنا بتنفيذ قيود خنق أكثر صرامة على تطبيقات الخلفية (الترحيل وDLP وحلول النسخ الاحتياطي) خلال ساعات النهار في أيام الأسبوع. يجب أن تتوقع أن تحقق هذه التطبيقات إنتاجية محدودة جدًا خلال هذه الأوقات. ومع ذلك ، خلال ساعات المساء وعطلة نهاية الأسبوع للمنطقة ، ستكون الخدمة جاهزة لمعالجة حجم أكبر بكثير من الطلبات من تطبيقات الخلفية.

**503 خادم خطأ مشغول**

قد يتلقى المستخدمون ملقم 503 خطأ مشغول عند محاولة الانتقال إلى مواقع SharePoint أو OneDrive. 

يمكن أن يكون سبب هذا الخطأ اختناق داخل خدمة SharePoint. يستخدم SharePoint Online الاختناق للحفاظ على الأداء الأمثل وموثوقية خدمة SharePoint Online. الاختناق يحد من عدد إجراءات المستخدم أو المكالمات المتزامنة (بواسطة البرنامج النصي أو التعليمات البرمجية) لمنع الإفراط في استخدام الموارد. 

لمزيد من المعلومات حول الاختناق انظر، [تجنب الحصول على خنق أو حظر في SharePoint عبر الإنترنت](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

إذا كنت تعتقد أن هذا الخطأ لا علاقة له بالاختناق، يمكنك التحقق مما إذا كانت هناك صيانة نشطة تحدث على المستأجر الخاص بك عن طريق التنقل إلى [مركز الرسائل](https://portal.office.com/adminportal/home#/MessageCenter).

 أخيرًا، تأكد من زيارة صفحة ["صحة الخدمة"](https://portal.office.com/adminportal/home#/servicehealth) للتحقق من أي تحذيرات/حوادث قد تحدث.

