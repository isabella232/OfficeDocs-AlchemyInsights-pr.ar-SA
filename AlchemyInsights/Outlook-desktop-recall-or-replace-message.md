---
title: برنامج Outlook لسطح المكتب لاستدعاء رسالة بريد الكتروني أو استبدالها
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663977"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>استدعاء رسالة بريد الكتروني في Outlook أو استبدالها

- بصفتك المسؤول ، يمكنك **استدعاء الرسائل بالنيابة عن المستخدمين الذين يستخدمون PowerShell**. لا يمكنك استدعاء الرسائل من مركز الاداره.
- يمكنك **فقط استدعاء الرسائل التي يتم إرسالها إلى الأشخاص في مؤسستك**. إذا تم إرسال الرسالة إلى عنوان Gmail ، علي سبيل المثال ، لا يمكنك استدعاؤها.
- يمكنك **فقط استدعاء الرسائل المرسلة من Outlook 2016 علي الكمبيوتر الشخصي**. إذا أرسل أحد المستخدمين رسالة باستخدام Outlook for Mac أو Outlook علي الويب ، فلا يمكنك استدعاؤه.

لاستدعاء رسالة بريد الكتروني أو استبدالها:

1. في جزء المجلدات الموجود في الجانب الأيمن من نافذه Outlook ، حدد مجلد العناصر المرسلة.
1. انقر نقرا مزدوجا فوق الرسالة التي تريد استدعاؤها لفتحها.
1. حدد علامة التبويب **رسالة** ، ثم حدد **الإجراءات**  >  **استدعاء هذه الرسالة**.
1. حدد **حذف النسخ غير المقروءة لهذه الرسالة** أو **حذف النسخ غير المقروءة واستبدالها برسالة جديده**، ثم حدد **موافق**.
1. إذا كنت ترسل رسالة بديله ، فقم بإنشاء الرسالة ، ثم حدد **إرسال**.
1. يتوقف نجاح أو فشل رسالة الاستدعاء علي إعدادات المستلم في Outlook. للاطلاع علي الخطوات المطلوبة للتحقق من الاستدعاء ، راجع [هذه المقالة](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

البحث عن رسائل البريد الكتروني وحذفها في مؤسستك

- إذا لم تكن مسؤولا عاما ، فيجب أضافه حسابك إلى دور أداره eDiscovery أو دور أداره البحث في التوافق للبحث عن الرسائل. لحذف الرسائل ، ستحتاج إلى الانضمام إلى مجموعه ادوار أداره المؤسسة أو البحث وأزاله دور الاداره. يتم تعيين الأذونات لهذه الأدوار في [مركز الأمان والتوافق](https://go.microsoft.com/fwlink/?linkid=2083731).
- [إنشاء بحث محتوي](https://docs.microsoft.com/microsoft-365/compliance/content-search) للعثور علي الرسالة التي تريد حذفها.
- [الاتصال بمركز التوافق والأمان PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

إذا كنت تستخدم مصادقه متعددة العوامل ، فراجع [الاتصال بمركز الأمان والتوافق في Microsoft 365 باستخدام مصادقه متعددة العوامل](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).