---
title: نقل رسائل البريد الكتروني إلى علبه بريد الأرشيف
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
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799767"
---
# <a name="move-email-to-the-archive-mailbox"></a>نقل البريد الكتروني إلى علبه بريد الأرشيف

إذا كنت تريد ان يقومنا بتشغيل التدقيق التلقائي للإعدادات المذكورة أدناه ، فحدد الزر السابق < وفي اعلي هذه الصفحة ، ثم ادخل عنوان البريد الكتروني للمستخدم الذي لديه مشاكل في نقل البريد الكتروني إلى علبه بريد الأرشيف الخاصة به.

1. تاكد من تمكين **علبه بريد الأرشيف** . إذا لم يكن كذلك ، فاستخدم الخطوات [المذكورة في هذه المقالة](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) لتمكين علبه بريد الأرشيف.

2. لأرشفه الرسائل تلقائيا إلى علبه بريد الأرشيف ، يجب تعيين علامة الاستبقاء التي تحتوي علي الاجراء **نقل إلى الارشفه** **تلقائيا إلى الوضع "التطبيق" علي علبه البريد بالبالكامل (افتراضي)**. استخدم الخطوات الواردة هنا لإنشاء العلامة: [أرشفه العلامة الافتراضية](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. بعد ذلك ، أضف علامة **الأرشيف** إلى نهج الاستبقاء. في مركز أداره Exchange ، اختر **نهج الاستبقاء** > أضف **علامة النقل إلى الأرشيف** إلى النهج ال> **حفظه**.

4. [الآن يمكنك تعيين نهج الاستبقاء](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) إلى علبه البريد الخاصة بالمستخدم المحدد. سيتم تطبيق نفس النهج علي كل من علبه البريد **الاساسيه** **والارشفه** .

قد يكون من الضروري فرض مساعد المجلد المدار (MFA) لتشغيل الإعدادات الجديدة وتطبيقها علي علبه بريد المستخدم. قم بتشغيل الأمر التالي اثناء [الاتصال ب أكسو PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) لبدء تشغيل مساعد المجلد المدار لعلبه بريد معينه:
  
بدء الماناجيدفولديراسيستانت-الهوية <name of the mailbox>

للحصول علي مزيد من المعلومات حول اعداد نهج أرشفه ، راجع اعداد [نهج الارشفه والحذف لعلب البريد](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  