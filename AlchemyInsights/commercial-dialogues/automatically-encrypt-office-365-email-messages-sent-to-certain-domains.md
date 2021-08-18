---
title: تشفير رسائل Office 365 الإلكتروني المرسلة إلى مجالات معينة تلقائيا
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: d30535d8605fcbfa0ca73c262d8f8671d73234a4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318835"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>تشفير رسائل Office 365 الإلكتروني المرسلة إلى مجالات معينة تلقائيا

1. من مركز [Exchange،](https://outlook.office365.com/ecp/)اختر **تدفق** البريد > قواعد . 
2. انقر فوق **الأيقونة جديد (+)،** ثم انقر فوق تطبيق تشفير الرسائل من Office 365 **وحماية الحقوق على الرسائل.**
3. في **الاسم**، أدخل اسما للقاعدة، مثل *تشفير الرسائل المرسلة* إلى contoso.com .
4. في **تطبيق هذه القاعدة إذا**، اختر المستلم > المجال **هو**. 
5. أدخل اسم المجال، مثل contoso.com **.**
6. انقر فوق **الأيقونة إضافة (+)،** ثم انقر فوق **موافق**.
7. إلى بجانب الحقل **قم بما يلي،** انقر **فوق تحديد واحد**. 
8. في القائمة **المنسدلة قالب RMS،** حدد **تشفير**، ثم انقر فوق **موافق**. (إذا لم تشاهد هذا الخيار، فهذا يعني أن خطتك لا تتضمن التشفير التلقائي. ولكن يمكنك إضافته!)
9. اختر أي تحديد اختياري (من قائمة التحديدات الاختيارية التي يمكنك إجراءها في هذه المرحلة، ويمكن ترك العديد منها مع الإعداد الافتراضي للتبسيط).
10. انقر فوق **حفظ**.

**هام**: يمكنك دائما الرجوع وتحرير هذه القاعدة لاحقا.

لمزيد من المعلومات حول إنشاء قواعد التشفير، راجع تعريف قواعد تدفق البريد [لتشفير](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) رسائل البريد الإلكتروني في Office 365