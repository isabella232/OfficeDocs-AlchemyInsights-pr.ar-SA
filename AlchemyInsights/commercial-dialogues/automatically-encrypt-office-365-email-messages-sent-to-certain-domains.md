---
title: تشفير رسائل البريد الإلكتروني ل Office 365 المرسلة إلى مجالات معينة تلقائيا
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743101"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>تشفير رسائل البريد الإلكتروني ل Office 365 المرسلة إلى مجالات معينة تلقائيا

1. من مركز [إدارة Exchange،](https://outlook.office365.com/ecp/)اختر **تدفق البريد > قواعد .** 
2. انقر فوق **الأيقونة جديد (+)،** ثم انقر فوق تطبيق تشفير الرسائل وحماية الحقوق في **Office 365 على الرسائل.**
3. في **الاسم**، أدخل اسما للقاعدة، مثل *تشفير الرسائل المرسلة إلى contoso.com*.
4. في **تطبيق هذه القاعدة إذا**، اختر المستلم > المجال **هو**. 
5. أدخل اسم المجال، مثل contoso.com **.**
6. انقر فوق **الأيقونة إضافة (+)،** ثم انقر فوق **موافق**.
7. إلى بجانب الحقل **قم بما يلي،** انقر **فوق تحديد واحد**. 
8. في القائمة **المنسدلة قالب RMS،** حدد **تشفير**، ثم انقر فوق **موافق**. (إذا لم تشاهد هذا الخيار، فهذا يعني أن خطتك لا تتضمن التشفير التلقائي. ولكن يمكنك إضافته!)
9. اختر أي تحديد اختياري (من قائمة التحديدات الاختيارية التي يمكنك إجراءها في هذه المرحلة، ويمكن ترك العديد منها مع الإعداد الافتراضي للتبسيط).
10. انقر فوق **حفظ**.

> [!IMPORTANT]
> يمكنك دائما الرجوع وتحرير هذه القاعدة لاحقا.

لمزيد من المعلومات حول إنشاء قواعد التشفير، راجع تعريف قواعد تدفق البريد لتشفير رسائل البريد الإلكتروني [في Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)