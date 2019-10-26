---
title: استدعاء سطح مكتب Outlook أو استبدال رسالة بريد الكتروني
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496098"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>استدعاء أو استبدال رسالة بريد الكتروني Outlook

- كما المشرف ، يمكنك **استدعاء الرسائل نيابة عن المستخدمين باستخدام PowerShell**. لا يمكنك تذكر الرسائل من مركز الاداره.
- يمكنك **فقط استدعاء الرسائل التي يتم إرسالها إلى الأشخاص في المؤسسة الخاصة بك**. إذا تم إرسال الرسالة إلى عنوان Gmail ، علي سبيل المثال ، لا يمكنك تذكر ذلك.
- يمكنك **فقط استدعاء الرسائل المرسلة من Outlook 2016 علي جهاز الكمبيوتر**. إذا قام مستخدم بإرسال رسالة باستخدام Outlook لنظام التشغيل Mac أو Outlook علي الويب ، لا يمكنك تذكر ذلك.

لاستدعاء رسالة بريد الكتروني أو استبدالها:

1. في جزء المجلد علي يسار اطار Outlook ، حدد مجلد "العناصر المرسلة".
1. انقر نقرا مزدوجا فوق الرسالة التي تريد استدعاءها لفتحها.
1. حدد علامة التبويب **رسالة** ثم حدد **الإجراءات** > **استدعاء هذه الرسالة**.
1. حدد **حذف النسخ غير المقروءة من هذه الرسالة** أو **احذف النسخ غير المقروءة واستبدلها برسالة جديده**، ثم حدد **موافق**.
1. إذا كنت ترسل رسالة بديله ، فقم بإنشاء الرسالة ، ثم حدد **إرسال**.
1. نجاح أو فشل استدعاء رسالة يعتمد علي إعدادات المستلم في Outlook. للحصول علي خطوات للتحقق من استدعاء ، راجع [هذه المقالة](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

البحث عن رسائل البريد الكتروني وحذفها في مؤسستك

- إذا لم تكن مسؤولا عموميا ، فيجب أضافه حسابك إلى دور مدير eDiscovery أو دور أداره بحث التوافق للبحث عن الرسائل. لحذف الرسائل ، ستحتاج إلى الانضمام إلى مجموعه دور أداره المؤسسة أو دور أداره البحث والازاله. يتم تعيين الأذونات لهذه الأدوار في [مركز الأمان والتوافق](https://go.microsoft.com/fwlink/?linkid=2083731).
- [إنشاء بحث محتوي](https://docs.microsoft.com/office365/securitycompliance/content-search) للعثور علي الرسالة التي تريد حذفها.
- [الاتصال بمركز الأمان والتوافق PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

إذا كنت تستخدم المصادقة متعددة العوامل ، راجع [الاتصال ب Office 365 الأمان ومركز التوافق PowerShell باستخدام مصادقه متعددة العوامل](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).