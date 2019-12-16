---
title: S/MIME في Outlook علي الويب
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053212"
---
# <a name="encrypt-email-messages-in-outlook"></a>تشفير رسائل البريد الكتروني في اوتلوك

تم بناء Office 365 تشفير الرسائل علي Microsoft Azure حقوق أداره (Azure RMS) ، وهو جزء من حماية المعلومات Azure. إذا كان الاشتراك الخاص بك يتضمن أداره حقوق Azure أو حماية معلومات Azure ، **لا تحتاج إلى اتخاذ إيه إجراءات لتمكين أو تنشيط** "خدمه أداره الحقوق" يدويا.

استنادا إلى ملاحظات العملاء ، لن نتمكن بعد الآن من تمكين قواعد تدفق بريد Exchange لتشفير البريد الكتروني الصادر تلقائيا الذي يحتوي علي نوع معين من المعلومات الحساسة في المستاجر بشكل افتراضي. بدلا من ذلك ، نحن نقدم تعليمات مفصله حول كيف يمكنك ان تفعل ذلك بأنفسكم. للحصول علي تفاصيل اضافيه حول كيفيه إنشاء قاعده نقل لتشفير المعلومات الحساسة ، راجع [هذه المقالة](https://aka.ms/OmeEtr).

- في حاله استخدام Outlook علي ويب ( **OWA**سابقا): عند إنشاء رسالة بريد الكتروني ، ببساطه انقر فوق **حماية** في OWA. سيتم تطبيق هذا الاذن "عدم الاعاده إلى الامام". انقر فوق **تغيير الاذن** واختر **تشفير** لتشفير الرسالة فقط.

- في حاله استخدام **عميل outlook**: لإرسال رسالة مشفره من outlook 2013 أو 2016 ، أو outlook 2016 لنظام التشغيل Mac ، حدد **أذونات الخيارات** > ****، ثم حدد خيار الحماية الذي تحتاجه.

- **لتشفير كافة البريد الكتروني** المرسلة إلى بعض المستلمين أو المؤسسات الشريكة الخارجية تلقائيا ، تحتاج إلى إنشاء قاعده نقل تدفق البريد في مركز مسؤول Exchange. يتم توفير تعليمات مفصله في [هذا المقال الدعم](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

