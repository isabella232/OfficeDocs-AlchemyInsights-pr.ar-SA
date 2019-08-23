---
title: نقل رسائل البريد الإلكتروني إلى أرشيف علبة البريد
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
ms.openlocfilehash: ce52df446fc4c23c06476e8836ade6a6810d158f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36548990"
---
# <a name="move-email-to-the-archive-mailbox"></a>نقل البريد الإلكتروني إلى أرشيف علبة البريد

1. تأكد من أن **أرشفة علبة البريد** تم تمكينه. إذا لم يكن الأمر كذلك، استخدام الخطوات الموجودة في [هذه المقالة](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) لتمكين علبة البريد الأرشيف.

2. لأرشفة الرسائل تلقائياً إلى أرشيف علبة البريد، يجب تعيين علامة استبقاء مع إجراء **نقل لأرشفة** تطبيقها **تلقائياً على علامة علبة البريد بالكامل (افتراضي)**. استخدم الخطوات هنا لإنشاء العلامة: ["الأرشيف الافتراضي" علامة](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).

3. بعد ذلك إضافة علامة **الأرشيف** إلى نهج استبقاء. في مركز مسؤول Exchange، اختيار **نهج الاستبقاء** إضافة **الانتقال إلى العلامة أرشيف** > إلى > نهج **حفظ**.

4. الآن [تعيين "نهج الاستبقاء"](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) لعلبة البريد لمستخدم معين. سيتم تطبيق نفس النهج **الأساسي** و **أرشيف** علبة البريد.

قد يكون من الضروري فرض إدارة مجلد مساعد (وزارة الخارجية) لتشغيل وتطبيق الإعدادات الجديدة بعلبة بريد مستخدم. تشغيل الأمر التالي أثناء [الاتصال ب PowerShell أكسو](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) لبدء إدارة "مساعد المجلدات" لعلبة بريد محددة:
  
ابدأ-ماناجيدفولديراسيستانت-الهوية<name of the mailbox>

لمزيد من المعلومات حول إعداد نهج أرشيف، راجع [إعداد نهج الأرشيف والحذف لعلب البريد](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  