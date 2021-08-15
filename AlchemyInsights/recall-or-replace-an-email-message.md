---
title: استدعاء رسالة بريد إلكتروني أو استبدالها
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024373"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>استدعاء رسالة بريد إلكتروني أو استبدالها في Microsoft 365

- يمكنك فقط **استدعاء الرسائل المرسلة** إلى أشخاص في مؤسستك . على سبيل المثال، إذا تم إرسال الرسالة إلى عنوان Gmail، لا يمكنك استدعاءها.
- يمكنك فقط استدعاء الرسائل المرسلة من Outlook **للكمبيوتر الشخصي**. إذا أرسل مستخدم رسالة باستخدام Outlook for Mac أو Outlook على ويب، لا يمكنك استدعاءها.
- كمسؤول مستأجر، يمكنك استدعاء الرسائل بالنيابة عن المستخدمين باستخدام **PowerShell** (لمزيد من المعلومات، راجع: البحث عن رسائل البريد الإلكتروني [وحذفها).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- لا يمكنك استدعاء الرسائل من مركز الإدارة. قم بالتمرير لأسفل وصولا إلى "البحث عن رسائل البريد الإلكتروني وحذفها في مؤسستك" للحصول على مزيد من المعلومات.

**استدعاء رسالة بريد إلكتروني أرسلتها أو استبدالها**

1. في جزء المجلد على الجانب الأيسر من نافذة Outlook، اختر المجلد العناصر المرسلة.
2. افتح الرسالة التي تريد استدعاءها. يجب النقر نقرا مزدوجا لفتح الرسالة. إن تحديد الرسالة بحيث تظهر في جزء القراءة لن يسمح لك باستدعاء الرسالة.
3. من علامة التبويب رسالة، حدد **إجراءات**  >  **استدعاء هذه الرسالة**.
4. اختر **حذف نسخ غير مقروءة** من هذه الرسالة أو حذف النسخ غير المقروءة واستبدالها برسالة **جديدة**، ثم حدد **موافق**.
5. إذا كنت ترسل رسالة بديلة، فحدد إنشاء الرسالة، ثم حدد **إرسال**.
6. يتوقف نجاح استدعاء رسالة أو فشله على إعدادات المستلمين في Outlook.

لمزيد من المعلومات، بما في ذلك كيفية التحقق من الاستدعاء، راجع استدعاء رسالة بريد إلكتروني أرسلتها أو [استبدالها](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***للبحث عن رسائل البريد*** الإلكتروني وحذفها في مؤسستك، يصبح الأمر أسهل إذا كنت مسؤول عام. إذا لم تكن المسؤول العام، فيجب إضافة حسابك إلى مجموعة دور مدير eDiscovery، أو إلى دور إدارة البحث في التوافق. لحذف الرسائل، ستحتاج إلى الانضمام إلى مجموعة دور إدارة المؤسسة أو دور إدارة البحث والحذف. يتم تعيين الأذونات لهذه الأدوار في مركز & [الأمان.](https://protection.office.com/)

1. [قم بإنشاء بحث في المحتوى](https://docs.microsoft.com/microsoft-365/compliance/content-search) للعثور على الرسالة التي تريد حذفها.
2. [الاتصال إلى الأمان & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

إذا كنت تستخدم المصادقة متعددة العوامل (المصادقة متعددة العوامل)، فشاهد الاتصال إلى Microsoft 365 الأمان & مركز التوافق [PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)باستخدام المصادقة متعددة العوامل .
