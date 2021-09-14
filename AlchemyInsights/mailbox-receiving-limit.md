---
title: فرض الحد الأقصى لعلبة البريد
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/31/2021
ms.locfileid: "59315769"
---
# <a name="mailbox-receiving-limit-enforcement"></a>فرض الحد الأقصى لعلبة البريد

بدأت Microsoft مؤخرا بفرض الحد لكل علبة بريد وهو 3600 رسالة في الساعة. لمزيد من المعلومات، [راجع Exchange Online الحدود.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits) Microsoft 365 علب البريد التي تتلقى أكثر من 3600 رسالة في غضون ساعة واحدة خلال ال 60 دقيقة القادمة. 

بالإضافة إلى ذلك، يتم تطبيق حد أزواج المرسلين والمستلمين (SRP) الذي يمنع الرسائل التي تستلمها علبة بريد Microsoft 365 من مرسل معين. إذا أرسل مرسل واحد أكثر من 33٪ من العتبة الإجمالية أو 1200 رسالة لكل ساعة درفلة إلى مستلم معين، يتم طرح حد SRP، ولا تقبل علبة البريد الرسائل الواردة من هذا المرسل. لاحظ ما يلي:

- يتم تطبيق هذا الحد على رسائل البريد الإلكتروني التي يتم تلقيها من مستأجرين آخرين أو مرسلين على الإنترنت.
- يتم حظر تسليم البريد الإلكتروني إلى علبة البريد خلال ال 60 دقيقة القادمة. 
- يتلقى المرسلون إلى علب البريد هذه تقريرا بعدم التسليم (5.2.121 أو 5.2.122) يفيد بأن علبة البريد تجاوزت الحد الأقصى لعتبة التسليم. يستمر تسليم البريد داخل المستأجر (البريد داخل المستأجر نفسه).
- عند تطبيق حد SRP، تستمر علبة البريد المستلمة في قبول الرسائل من مرسلين آخرين.

يمكن للمسؤولين مراقبة نشاط علبة البريد الحالية من خلال الوصول إلى تقرير جديد والوصول إلى معلومات متعمقة جديدة في مركز إدارة Exchange يسمى "تتجاوز علب البريد حدود التلقي". تظهر المعرفة فقط إذا كان المستأجر لديه علب بريد غير مسيئة، بينما يظهر التقرير دائما في لوحة المعلومات ولكنه فارغ إلا إذا كان المستأجر لديه علب بريد غير مهينة.

لمزيد من المعلومات حول حدود تلقي المعلومات، راجع علب البريد التي تتجاوز حدود تلقي المعرفة في [EAC الجديد](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights).

لمزيد من المعلومات حول تقرير تجاوز حدود التلقي، راجع علب البريد التي تتجاوز تقرير حدود التلقي [في EAC الجديد](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report).