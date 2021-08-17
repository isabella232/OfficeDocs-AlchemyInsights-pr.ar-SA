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
ms.openlocfilehash: 57a1756787f8297a2a1ab3012b95aaa2f33e6045
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313006"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>تحديد عنوان IP والعميل في سجلات التدقيق

يظهر عنوان IP الذي يتطابق مع نشاط Microsoft 365 المستخدم أو المسؤول في سجلات التدقيق. يتم أيضا تسجيل معلومات العميل. فيما يلي الخطوات اللازمة لتحديد مثل هذه المعلومات

1. سجل دخولك إلى Microsoft 365 [التوافق.](https://protection.office.com/)

2. انتقل إلى صفحة **البحث**  >  **في سجل تدقيق** البحث.

   إذا كنت مهتما بنشاط معين، فحدده من **قائمة** الأنشطة. إذا لم يكن الأمر كذلك، سيتم إرجاع كل الأنشطة للمستخدم المحدد (الإعداد الافتراضي).

   **ملاحظة:** قد لا تتوفر بعض الأنشطة في **قائمة الأنشطة؛** ومع ذلك، سيتم إرجاع عناصر التدقيق هذه إذا تم تحديد **إظهار** النتائج لكل الأنشطة (إعداد افتراضي).

3. حدد اسم المستخدم في الحقل **المستخدمون،** وحدد نطاق التاريخ المناسب للنشاط، ثم انقر فوق **بحث**.

في النتائج، يمكنك رؤية عنوان IP لهذا النشاط في جزء النتائج. حدد سجل التدقيق لرؤية معلومات  تفصيلية في قائمة التفاصيل من خلال قائمة منتحلة (على سبيل المثال، العميل، المستخدم الذي قام بتنفيذ الإجراء، وما إلى ذلك).

لمزيد من المعلومات، راجع [البحث عن عنوان IP للكمبيوتر المستخدم للوصول إلى حساب م اختراق](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
