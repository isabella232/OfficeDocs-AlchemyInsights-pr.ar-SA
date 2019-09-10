---
title: نقل رسائل البريد الإلكتروني إلى علبة بريد الأرشيف
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822149"
---
# <a name="move-email-to-the-archive-mailbox"></a>نقل البريد الإلكتروني إلى صندوق بريد الأرشيف

1. تأكد من تمكين **علبة بريد أرشيف.** إذا لم يكن الأمر كذلك، اتبع الخطوات المذكورة في [هذه المقالة](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) لتمكين علبة بريد الأرشيف.

2. لأرشفة الرسائل تلقائيًا إلى علبة بريد الأرشيف، يجب تعيين علامة استبقاء مع إجراء **النقل إلى الأرشيف** ليتم **تطبيقها تلقائيًا على علامة علبة البريد بأكملها (افتراضية).** استخدم الخطوات هنا لإنشاء العلامة: [أرشفة العلامة الافتراضية](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. بعد ذلك، أضف علامة **الأرشيف** إلى نهج الاستبقاء. في مركز مسؤول Exchange، اختر **نُهج الاستبقاء** > إضافة **علامة نقل إلى الأرشيف** إلى النهج > **حفظ**.

4. الآن [تعيين "نهج الاستبقاء"](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) إلى علبة بريد المستخدم المحدد. سيتم تطبيق نفس النهج على كل من علبة البريد **الأساسية** **والأرشيف.**

قد يكون من الضروري فرض "مساعد المجلدات المدارة" (MFA) لتشغيل وتطبيق الإعدادات الجديدة على علبة بريد المستخدم. قم بتشغيل الأمر التالي أثناء [الاتصال بـ EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) لبدء تشغيل "مساعد المجلدات المدارة" لعلبة بريد معينة:
  
بدء مُدارفولديرمساعد-الهوية<name of the mailbox>

لمزيد من المعلومات حول إعداد نهج أرشيف، راجع [إعداد نهج أرشفة وحذف لعلب البريد](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  