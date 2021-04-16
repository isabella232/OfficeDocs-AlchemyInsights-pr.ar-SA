---
title: هل تلقى المستخدمون بريدا إلكترونيا ضارا
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 425f9ba488fd69b8c5ea29636bccccd995bf48fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815233"
---
# <a name="did-your-users-receive-malicious-email"></a>هل تلقى المستخدمون بريدا إلكترونيا ضارا؟

- يمكنك الآن الإبلاغ عن البريد الإلكتروني الضار إلى Microsoft باستخدام إرسالات المسؤول [في مركز & التوافق.](https://sip.protection.office.com/reportsubmission)

يتم فحص الرسائل [](https://sip.protection.office.com/reportsubmission) التي يتم إرسالها في إرسالات المسؤول، كما تظهر النتائج التالية في القائمة **من** خلال التفاصيل:

- إذا كان هناك فشل في مصادقة البريد الإلكتروني للمرسل في وقت التسليم.
- معلومات حول أي من رسائل النهج التي قد تؤثر على قرار الرسالة أو تطغى عليه.
- نتائج الاحتواء الحالية لمعرفة ما إذا كانت عناوين URL أو الملفات المضمنة في الرسالة ضارة أم لا.
- ملاحظات من طلاب الدرجات

إذا تم العثور على تجاوز، يجب أن تكتمل عملية إعادة التجاوز خلال عدة دقائق. إذا لم تكن هناك مشكلة في مصادقة البريد الإلكتروني أو إذا لم يتأثر التسليم بتجاوز، فإن ملاحظات طلاب الدرجات قد تستغرق ما يصل إلى يوم واحد.

إذا كنت لا توافق على الحكم النهائي على رسالة أو عنوان URL أو ملف (تم حظره في مقابل لم يتم حظره)، ف أرسل الرسالة مرة أخرى بعد يوم لإعادة االرسالة. هناك احتمال كبير بأن يتم تغيير الحكم بعد إرسال الرسالة مرة أخرى.

في هذه الأثناء، يمكنك إزالة البريد الإلكتروني الضار من علبة الوارد الخاصة بالمستخدم باتباع الإرشادات الواردة [في هذه المقالة](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- يمكن للعملاء الذين تم استخدام Microsoft Defender ل Office 365 القيام ب:
    - استخدام ["مستكشف التهديدات" للعثور على البريد الإلكتروني المريب وحذفه](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [استخدام الارتباطات الآمنة لحظر الوصول إلى](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) عنوان URL ضار
    - تعقب المستخدمين الذين نقروا فوق عناوين URL الضارة والوصول إليها: [عرض عنوان URL](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)التصيد الاحتيالي والنقر فوق بيانات قرار الحصول على  &  [UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - بدء ["التحقيق التلقائي" يدويا](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

يمكنك أيضا الحماية من الملفات الضارة أو عناوين URL باتباع الإرشادات الواردة في الحماية من عناوين [URL والملفات الضارة.](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)