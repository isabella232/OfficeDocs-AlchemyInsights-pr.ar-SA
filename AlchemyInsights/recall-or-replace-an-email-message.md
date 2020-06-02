---
title: استدعاء رسالة بريد إلكتروني أو استبدالها
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509443"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>استدعاء رسالة بريد إلكتروني أو استبدالها في Microsoft 365

- يمكنك **فقط تذكر الرسائل التي يتم إرسالها إلى الأشخاص في مؤسستك.** إذا تم إرسال الرسالة إلى عنوان Gmail، على سبيل المثال، فلا يمكنك تذكرها.
- يمكنك **فقط تذكر الرسائل المرسلة من Outlook 2016 للكمبيوتر**. إذا أرسل مستخدم رسالة باستخدام Outlook for Mac أو Outlook على الويب، فلا يمكنك تذكرها.
- إذا كنت مسؤولاً، يمكنك **استدعاء الرسائل نيابة عن المستخدمين باستخدام PowerShell**. لا يمكنك تذكر الرسائل من مركز الإدارة. مرر لأسفل إلى "البحث عن رسائل البريد الإلكتروني وحذفها في مؤسستك" للحصول على مزيد من المعلومات.

**استدعاء رسالة بريد إلكتروني أرسلتها أو استبدالها**

1. في جزء المجلد الموجود على يسار إطار Outlook، اختر مجلد العناصر المرسلة.
2. افتح الرسالة التي تريد تذكرها. يجب النقر نقراً مزدوجاً لفتح الرسالة. لن يسمح لك تحديد الرسالة بحيث تظهر في جزء القراءة بتذكر الرسالة.
3. من علامة التبويب الرسالة، حدد **الإجراءات**  >  **استدعاء هذه الرسالة**.
4. اختر **حذف نسخ غير مقروءة من هذه الرسالة** أو حذف النسخ غير **المقروءة واستبدالها برسالة جديدة**، ثم حدد **موافق**.
5. إذا كنت ترسل رسالة بديلة، فقم بإنشاء الرسالة، ثم حدد **إرسال**.
6. يعتمد نجاح أو فشل استدعاء رسالة على إعدادات المستلمين في Outlook.

لمزيد من المعلومات، بما في ذلك كيفية التحقق من الاستدعاء، راجع [استدعاء أو استبدال رسالة بريد إلكتروني أرسلتها](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***البحث عن رسائل البريد الإلكتروني وحذفها في مؤسستك*** للبحث عن رسائل البريد الإلكتروني وحذفها في مؤسستك، يكون الأمر أسهل إذا كنت مسؤولاً عالمياً. إذا لم تكن مسؤولاً عمومياً، يجب إضافة حسابك إلى مجموعة أدوار مدير eDiscovery، أو إلى دور إدارة بحث التوافق. لحذف الرسائل، ستحتاج إلى الانضمام إلى مجموعة أدوار إدارة المؤسسة أو دور إدارة البحث والتطهير. يتم تعيين أذونات لهذه الأدوار في [مركز التوافق & الأمان](https://protection.office.com/).

1. [إنشاء بحث محتوى](https://docs.microsoft.com/microsoft-365/compliance/content-search) للعثور على الرسالة لحذفها.
2. [الاتصال بالأمان & مركز الامتثال PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)مركز . 

إذا كنت تستخدم MFA، راجع [الاتصال بأمان Microsoft 365 & مركز التوافق PowerShell باستخدام المصادقة متعددة العوامل](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
