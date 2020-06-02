---
title: تحديد إعادة توجيه البريد الإلكتروني الخارجي على صناديق البريد في سجلات التدقيق
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508939"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>تحديد وقت تكوين إعادة توجيه البريد الإلكتروني الخارجي على صناديق البريد

عندما يقوم مستخدم Microsoft 365 بتكوين إعادة توجيه البريد الإلكتروني الخارجي على علبة بريد، يتم تدقيق النشاط كجزء من **cmdlet Set-علبة البريد.** يمكنك مشاهدة النشاط باستخدام بحث سجل التدقيق في مركز التوافق & الأمان.

1. تسجيل الدخول إلى [مركز التوافق & الأمان Microsoft 365](https://protection.office.com/).

2. انتقل إلى **Search**صفحة البحث في  >  **سجل تدقيق** البحث.

3. حدد نطاق التاريخ في **حقول تاريخ البدء** وتاريخ **الانتهاء.** لا تحتاج إلى تحديد اسم مستخدم. تحقق من تعيين حقل **الأنشطة** **لإظهار النتائج لكافة الأنشطة**.

4. انقر فوق **البحث**.

في النتائج، انقر فوق **نتائج التصفية** واكتب **تعيين علبة البريد** في مربع عامل تصفية النشاط. حدد سجل تدقيق في النتائج. في **التفاصيل** المنبثقة، انقر فوق **مزيد من المعلومات**. يجب عليك الاطلاع على تفاصيل كل سجل تدقيق لتحديد ما إذا كان النشاط مرتبطًا بإعادة توجيه البريد الإلكتروني.

- **ObjectId:** قيمة الاسم المستعار لصندوق البريد الذي تم تعديله.

- **المعلمات**: _يشير إعادة توجيه SmtpAddress_ إلى عنوان البريد الإلكتروني المستهدف.

- **معرف المستخدم:** المستخدم الذي قام بتكوين إعادة توجيه البريد الإلكتروني على علبة البريد في حقل **ObjectId.**

لمزيد من المعلومات، راجع [تحديد من قام بإعداد إعادة توجيه البريد الإلكتروني لعلبة بريد](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
