---
title: تحديد عنوان IP والعميل في سجلات التدقيق
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668297"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>تحديد عنوان IP والعميل في سجلات التدقيق

يظهر عنوان IP المتوافق مع نشاط بواسطة مستخدم أو مسؤول Microsoft 365 في سجلات التدقيق. يتم أيضا تسجيل معلومات العميل. اليك الخطوات المطلوبة لتعريف هذه المعلومات

1. سجل الدخول إلى [مركز توافق & أمان Microsoft 365](https://protection.office.com/).

2. انتقل إلى صفحه **Search**  >  **البحث في سجل تدقيق** البحث.

   إذا كنت مهتما بنشاط معين ، فحدده من قائمه **الانشطه** . إذا لم يكن كذلك ، سيتم إرجاع كل الانشطه للمستخدم المحدد (الاعداد الافتراضي).

   **ملاحظه**: قد لا تتوفر بعض الانشطه في قائمه " **الانشطه** " ؛ ومع ذلك ، سيتم إرجاع عناصر التدقيق هذه إذا تم تحديد **إظهار النتائج لكل الانشطه** (الاعداد الافتراضي).

3. حدد اسم المستخدم في الحقل **المستخدمون** ، وحدد نطاق التاريخ المناسب للنشاط ، ثم انقر فوق **بحث**.

في النتائج ، يمكنك رؤية عنوان IP لهذا النشاط في جزء النتائج. حدد سجل التدقيق للاطلاع علي معلومات مفصله في القائمة المنبثقة **التفاصيل** (علي سبيل المثال ، العميل والمستخدم الذي نفذ الاجراء ، وما إلى ذلك).

للحصول علي مزيد من المعلومات ، راجع [البحث عن عنوان IP الخاص بالكمبيوتر المستخدم للوصول إلى حساب اختراق](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
