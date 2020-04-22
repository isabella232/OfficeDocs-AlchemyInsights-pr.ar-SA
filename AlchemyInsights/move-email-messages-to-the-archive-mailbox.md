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
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713633"
---
# <a name="move-email-to-the-archive-mailbox"></a>نقل البريد الإلكتروني إلى صندوق بريد الأرشيف

1. تأكد من تمكين **علبة بريد أرشيف.** إذا لم يكن كذلك، استخدم الخطوات في [هذه المقالة](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) لتمكين علبة بريد الأرشيف.

2. لأرشفة الرسائل تلقائيًا إلى صندوق بريد الأرشيف، يجب تعيين علامة الاحتفاظ مع إجراء **النقل إلى الأرشيف** ليتم تطبيقها **تلقائيًا على علامة علبة البريد بأكملها (الافتراضية).** استخدم الخطوات هنا لإنشاء العلامة: [علامة الأرشيف الافتراضية](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. بعد ذلك، أضف علامة **الأرشيف** إلى سياسة الاحتفاظ. في مركز إدارة Exchange، اختر **نُهج الاحتفاظ** > إضافة **علامة الانتقال إلى الأرشيف** إلى النهج > **حفظ**.

4. الآن [تعيين نهج الاحتفاظ](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) إلى علبة بريد المستخدم معينة. سيتم تطبيق نفس النهج على كل من **علبة** البريد الأساسية **وعلبة البريد الأرشيف.**

قد يكون من الضروري فرض "مساعد المجلد المدارة" (MFA) لتشغيل وتطبيق الإعدادات الجديدة على علبة بريد المستخدم. تشغيل الأمر التالي أثناء [الاتصال بـ EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) لبدء تشغيل "مساعد المجلد المدار" لعلبة بريد معينة:
  
بدء إدارة FolderedAssistant -الهوية<name of the mailbox>

لمزيد من المعلومات حول إعداد نهج أرشيف، راجع [إعداد نهج أرشيف وحذف لصناديق البريد](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  