---
title: نقل رسائل البريد الإلكتروني إلى صندوق بريد الأرشيف
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522758"
---
# <a name="move-email-to-the-archive-mailbox"></a>نقل البريد الإلكتروني إلى صندوق بريد الأرشيف

إذا كنت تريد منا تشغيل الشيكات التلقائية للإعدادات المذكورة أدناه، حدد زر العودة <- في الجزء العلوي من هذه الصفحة، ومن ثم أدخل عنوان البريد الإلكتروني للمستخدم الذي لديه مشاكل في نقل البريد الإلكتروني إلى صندوق بريد الأرشيف الخاصة بهم.

1. تأكد من تمكين **علبة بريد أرشيف.** إذا لم يكن كذلك، استخدم الخطوات المذكورة في [هذه المقالة](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) لتمكين علبة البريد الأرشيف.

2. لأرشفة الرسائل تلقائيًا إلى صندوق بريد الأرشيف، يجب تعيين علامة الاحتفاظ مع إجراء **النقل إلى الأرشيف** **لتطبيقها تلقائيًا على علامة علبة البريد بأكملها (افتراضي).** استخدم الخطوات هنا لإنشاء العلامة: [وضع علامة الأرشفة الافتراضية](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. بعد ذلك، أضف علامة **الأرشيف** إلى نهج الاستبقاء. في مركز مسؤول Exchange، اختر **نُهج الاستبقاء** > إضافة **علامة نقل إلى الأرشيف** إلى النهج > **حفظ**.

4. الآن [تعيين نهج الاستبقاء](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) إلى علبة بريد المستخدم معينة. سيتم تطبيق نفس النهج على كل من صندوق البريد **الأساسي** و **"الأرشيف".**

قد يكون من الضروري فرض "مساعد المجلد المدارة" (MFA) لتشغيل وتطبيق الإعدادات الجديدة إلى علبة البريد الخاصة بالمستخدم. تشغيل الأمر التالي أثناء [الاتصال بـ EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) لبدء تشغيل "مساعد المجلد المُدار" لعلبة بريد معينة:
  
بدء-مدارةمبدأاًمبدأاً -هوية<name of the mailbox>

لمزيد من المعلومات حول إعداد نهج أرشيف، راجع [إعداد نهج الأرشفة والحذف لصناديق البريد](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  