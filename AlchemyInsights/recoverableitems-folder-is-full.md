---
title: 1336 مجلد RecoverableItems ممتلئ
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061743"
---
# <a name="the-recoverable-items-folder-is-full"></a>مجلد "العناصر القابلة لاسترداده" ممتلئ

بالنسبة Exchange Online علب البريد، يكون حد التخزين الافتراضي لمجلد "العناصر القابلة لاستردادها" هو 30 غيغابايت. يزيد الحد الأقصى للتخزين لمجلد العناصر القابلة لاسترداده تلقائيا إلى 100 غيغابايت إذا تم وضع علبة البريد في الاحتجاز بسبب الدعاوى القضائية أو احتجاز eDiscovery أو تم تعيينها إلى نهج استبقاء.

عندما يصل مجلد العناصر القابلة لاستردادها إلى الحد الأقصى للتخزين، تتأثر وظائف علبة البريد باتباع الطرق التالية:

- لا يمكن للمستخدم حذف العناصر من علبة البريد.

- لا يمكن لمساعد المجلد المدار حذف العناصر استنادا إلى علامة الاستبقاء أو إعدادات المجلدات المدارة.

- بالنسبة إلى علب البريد التي تم تمكين "استرداد عنصر واحد" لها أو التي تم وضعها قيد الانتظار، لا يمكن لعملية حماية صفحة النسخ عند الكتابة الاحتفاظ بنسخ من العناصر التي قام المستخدم بتحريرها.

- بالنسبة لعلب البريد التي تم تمكين "تسجيل تدقيق علبة البريد"، لا يمكن حفظ إدخالات سجل تدقيق علبة البريد في المجلد الفرعي "عمليات التدقيق" في مجلد "العناصر القابلة للاسترداد".

بالنسبة لعلب البريد غير الموقوقة، يمكن للمسؤولين استخدام الأمر في Exchange Online PowerShell لحذف العناصر الموجودة في مجلد العناصر القابلة `Search-Mailbox -SearchDumpsterOnly -DeleteContent` لاستردادها. لمزيد من المعلومات، راجع المواضيع التالية:

- [البحث عن الرسائل وحذفها](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

بالنسبة لعلب البريد الموقوفة، يجب على المسؤولين إزالة الانتظار قبل أن يمكنهم حذف العناصر من مجلد العناصر القابلة للاسترداد. لمزيد من المعلومات، راجع حذف العناصر في مجلد العناصر القابلة لاسترداد علب البريد المستندة إلى السحابة [في الانتظار](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

للمساعدة على منع مجلد "العناصر القابلة للاسترداد" من أن يصبح كاملا، يمكن للمسؤولين زيادة الحد الأقصى للتخزين في مجلد "العناصر القابلة لاسترداد" لعلب البريد الموقتة، كما يمكنهم إعداد نهج استبقاء لعلبة البريد ينقل العناصر من مجلد "العناصر القابلة لاستردادها" إلى علبة بريد الأرشيف الخاصة بالمستخدم. راجع [زيادة الحصة النسبية للعناصر القابلة للاسترداد لعلب البريد الموقوقة](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
