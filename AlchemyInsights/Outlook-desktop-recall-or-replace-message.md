---
title: Outlook استدعاء رسالة بريد إلكتروني أو استبدالها على سطح المكتب
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
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918382"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>استدعاء رسالة بريد إلكتروني Outlook بريد إلكتروني أو استبدالها

- ب أنت المسؤول، يمكنك استدعاء الرسائل نيابة **عن المستخدمين الذين يستخدمون PowerShell**. لا يمكنك استدعاء الرسائل من مركز الإدارة.
- يمكنك فقط **استدعاء الرسائل المرسلة** إلى أشخاص في مؤسستك . إذا تم إرسال الرسالة إلى عنوان Gmail، على سبيل المثال، لا يمكنك استدعاءها.
- يمكنك فقط **استدعاء الرسائل المرسلة من** Outlook 2016 على الكمبيوتر الشخصي . إذا أرسل مستخدم رسالة باستخدام Outlook for Mac أو Outlook على ويب، لا يمكنك استدعاءها.

لاستدعاء رسالة بريد إلكتروني أو استبدالها:

1. في جزء المجلد على الجانب الأيسر من نافذة Outlook، حدد المجلد العناصر المرسلة.
1. انقر نقرا مزدوجا فوق الرسالة التي تريد استدعاءها لفتحها.
1. حدد علامة **التبويب رسالة،** ثم حدد **إجراءات**  >  **استدعاء هذه الرسالة**.
1. حدد **حذف النسخ غير المقروءة** من هذه الرسالة أو **حذف** النسخ غير المقروءة واستبدالها برسالة جديدة ، ثم حدد **موافق**.
1. إذا كنت ترسل رسالة بديلة، فحدد إنشاء الرسالة، ثم حدد **إرسال**.
1. يعتمد نجاح استدعاء رسالة أو فشله على إعدادات المستلم في Outlook. للحصول على خطوات للتحقق من الاستدعاء، راجع [هذه المقالة](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

البحث عن رسائل البريد الإلكتروني وحذفها في مؤسستك

- إذا لم تكن المسؤول العام، فيجب إضافة حسابك إلى دور eDiscovery Manager أو دور إدارة البحث في التوافق للبحث عن الرسائل. لحذف الرسائل، ستحتاج إلى الانضمام إلى مجموعة دور إدارة المؤسسة أو دور إدارة البحث والحذف. يتم تعيين الأذونات لهذه الأدوار في [مركز الأمان والتوافق](https://go.microsoft.com/fwlink/?linkid=2083731).
- [قم بإنشاء بحث في المحتوى](https://docs.microsoft.com/microsoft-365/compliance/content-search) للعثور على الرسالة التي تريد حذفها.
- [الاتصال إلى مركز الأمان والتوافق PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

إذا كنت تستخدم مصادقة متعددة العوامل، الاتصال إلى Microsoft 365 مركز التوافق والأمان [PowerShell باستخدام المصادقة متعددة العوامل](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).