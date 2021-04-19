---
title: استخدام DLP في قواعد النقل
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827203"
---
# <a name="using-dlp-in-transport-rules"></a>استخدام DLP في قواعد النقل

لدمج تفادي فقدان البيانات (DLP) في عملية نقل موجودة، استخدم الشرط "**إذا كانت الرسالة تحتوي على...المعلومات الحساسة**" في إعداد قاعدة النقل.

**لمزيد من التفاصيل، اطلع على:**

- أنواع المعلومات الحساسة لتقنية DLP المتكاملة في قواعد النقل: [تكامل قواعد المعلومات الحساسة](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

يمكنك أيضاً اختبار القاعدة باستخدام اختبار النهج أو بدونه باستخدام "وضع الاختبار" على القاعدة.  يجب الانتظار 30 دقيقة بعد إنشاء القاعدة قبل اختبارها.

- راجع [اختبار قواعد تدفق/نقل البريد](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**ملاحظة**: إذا كنت تحاول تنفيذ نهج DLP جديد باستخدام قواعد النقل في EAC، فاستخدم [نهج DLP في مركز التوافق والأمان](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) بدلاً من ذلك.
