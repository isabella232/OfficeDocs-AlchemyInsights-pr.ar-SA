---
title: استدعاء outlook سطح المكتب أو استبدال رسالة بريد إلكتروني
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: aad9f863bc9fd7d5522c480bd1a7d15f3a80ff4f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/15/2019
ms.locfileid: "30657031"
---
# <a name="recall-or-replace-an-email-message"></a>استرداد أو استبدال رسالة بريد إلكتروني

- كالمسؤول، يمكنك **استدعاء الرسائل بالنيابة عن المستخدمين استخدام PowerShell**. لا يمكن استدعاء الرسائل من مركز الإدارة.
- يمكنك **فقط استدعاء الرسائل التي يتم إرسالها إلى الأشخاص الموجودين في مؤسستك**. إذا تم إرسال الرسالة إلى عنوان Gmail، على سبيل المثال، تتمكن من استرداده.
- يمكنك **فقط استدعاء الرسائل المرسلة من 2016 Outlook على جهاز الكمبيوتر**. إذا كان مستخدم إرسال رسالة باستخدام Outlook لنظام التشغيل Mac أو Outlook على الويب، تتمكن من استرداده.

لاسترداد أو استبدال رسالة بريد إلكتروني:

1. في جزء المجلدات في الجزء الأيمن من إطار Outlook، حدد مجلد "العناصر المرسلة".
1. انقر نقراً مزدوجاً فوق الرسالة التي تريد استدعائها لفتحها.
1. حدد علامة التبويب **رسالة** ، وحدد **إجراءات** > **استدعاء هذه الرسالة**.
1. حدد **حذف النسخ غير المقروءة من هذه الرسالة** أو **حذف النسخ غير المقروءة واستبدالها برسالة جديدة**، ومن ثم حدد **"موافق"**.
1. إذا كنت ترسل رسالة استبدال، إنشاء الرسالة وقم **إرسال**.
1. نجاح أو فشل استدعاء الرسالة يعتمد على إعدادات المستلم في Outlook. لمزيد من الخطوات للتحقق من الاسترداد، راجع [هذا المقال](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

البحث عن وحذف رسائل البريد الإلكتروني في مؤسستك

- إذا لم تكن إدارة عمومية، يجب إضافة الحساب إلى دور إدارة eDiscovery أو دور إدارة "التوافق البحث" للبحث عن الرسائل. لحذف الرسائل، سوف تحتاج إلى الانضمام إلى مجموعة "إدارة المؤسسة" دور أو أدوار إدارة البحث وإزالة. يتم تعيين الأذونات لهذه الأدوار في [مركز الأمان والتوافق](https://go.microsoft.com/fwlink/?linkid=2083731).
- [إنشاء محتوى البحث](https://docs.microsoft.com/office365/securitycompliance/content-search) للعثور على الرسالة لحذف.
- [الاتصال بأمان و PowerShell مركز التوافق](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

إذا كنت تستخدم مصادقة متعددة العوامل، راجع [الاتصال ب Office 365 الأمان والتوافق PowerShell مركز استخدام مصادقة متعددة العوامل](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).