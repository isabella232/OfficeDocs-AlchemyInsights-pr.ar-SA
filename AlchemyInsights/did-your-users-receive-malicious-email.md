---
title: هل تلقى المستخدمون بريدا إلكترونيا ضارا
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291779"
---
# <a name="did-your-users-receive-malicious-email"></a>هل تلقى المستخدمون بريدا إلكترونيا ضارا؟

- يمكنك الآن الإبلاغ عن البريد الإلكتروني الضار إلى Microsoft باستخدام "إرسالات المسؤول" [في مركز التوافق & الأمان.](https://sip.protection.office.com/reportsubmission)

يتم فحص الرسائل [](https://sip.protection.office.com/reportsubmission) المرسلة في إرسالات المسؤول، كما يتم عرض النتائج التالية في **القائمة من خلال القائمة من القائمة من خلال** التفاصيل:

- في حالة حدوث فشل في مصادقة البريد الإلكتروني للمرسل في وقت التسليم.
- معلومات حول أي نهج قد يؤثر على قرار الرسالة أو يتجاوزه.
- نتائج الاحتواء الحالية لمعرفة ما إذا كانت عناوين URL أو الملفات المضمنة في الرسالة ضارة أم لا.
- ملاحظات من طلاب الدرجات

إذا تم العثور على تجاوز، يجب أن تكتمل عملية إعادة التجاوز في عدة دقائق. إذا لم تكن هناك مشكلة في مصادقة البريد الإلكتروني أو إذا لم يتأثر التسليم بتجاوز، يمكن أن تستغرق ملاحظات الدرجات حتى يوم واحد.

إذا لم توافق على القرار النهائي على رسالة أو عنوان URL أو ملف (تم حظره مقابل عدم حظره)، أرسل الرسالة مرة أخرى بعد يوم لإعادة البحث. هناك احتمال كبير بأن يتغير القرار بعد إرسال الرسالة مرة أخرى.

في هذه الأثناء، يمكنك إزالة البريد الإلكتروني الضار من علبة الوارد الخاصة بالمستخدمين باتباع الإرشادات الواردة [في هذه المقالة.](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)

- يمكن للعملاء الذين تم استخدام Microsoft Defender ل Office 365 القيام ب:
    - استخدام [Threat Explorer للعثور على البريد الإلكتروني المريب وحذفه](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [استخدام الارتباطات الآمنة لحظر الوصول](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) إلى عنوان URL ضار
    - تعقب المستخدمين الذين نقروا فوق عناوين URL الضارة والوصول إليها: عرض عنوان URL التصيد الاحتيالي والنقر فوق [بيانات قرار الحصول](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)على  &  [UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - بدء ["التحقيق التلقائي" يدويا](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

يمكنك أيضا الحماية من الملفات الضارة عناوين URL ومن خلال اتباع الإرشادات الواردة في "الحماية من عناوين [URL والملفات الضارة".](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)