---
title: نقل رسائل البريد الإلكتروني إلى علبة بريد الأرشيف
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974944"
---
# <a name="move-email-to-the-archive-mailbox"></a>نقل البريد الإلكتروني إلى علبة بريد الأرشيف

إذا كنت تريد منا تشغيل عمليات التحقق التلقائية من الإعدادات المذكورة أدناه، فحدد زر الخلف <-- في أعلى هذه الصفحة، ثم أدخل عنوان البريد الإلكتروني للمستخدم الذي يواجه مشاكل في نقل البريد الإلكتروني إلى علبة بريد الأرشيف الخاصة به.

1. تأكد من تمكين علبة بريد **الأرشيف.** إذا لم يكن الأمر كذلك، فاستخدم الخطوات الواردة [في هذه المقالة](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) لتمكين علبة بريد الأرشيف.

2. لأرشفة الرسائل تلقائيا إلى علبة بريد الأرشيف، يجب تعيين علامة استبقاء مع الإجراء **نقل** إلى الأرشيف إلى تطبيقها تلقائيا على علامة علبة البريد **بأكملها (افتراضيا).** استخدم الخطوات هنا لإنشاء العلامة: [أرشفة العلامة الافتراضية](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. بعد ذلك، أضف علامة **الأرشيف** إلى نهج الاستبقاء. في مركز Exchange، اختر نهج  الاستبقاء > إضافة علامة **نقل** إلى الأرشيف إلى نهج > **حفظ**.

4. الآن [قم بتعيين نهج الاستبقاء](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) إلى علبة بريد المستخدم المحدد. سيتم تطبيق النهج نفسه على كل من علبة **البريد الأساسية** **والأرشفة.**

قد يكون من الضروري إجبار مساعد المجلد المدار (MFA) على تشغيل الإعدادات الجديدة وتطبيقها على علبة بريد المستخدم. تشغيل الأمر التالي أثناء [الاتصال ب EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) لبدء تشغيل "مساعد المجلد المدار" لعلبة بريد معينة:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

لمزيد من المعلومات حول إعداد نهج أرشيف، راجع إعداد نهج أرشيف [وحذف لعلب البريد](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  