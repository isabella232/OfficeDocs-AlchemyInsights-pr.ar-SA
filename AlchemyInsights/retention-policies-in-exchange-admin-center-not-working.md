---
title: نهج الاستبقاء في مركز أداره Exchange لا تعمل
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740497"
---
# <a name="retention-policies-in-exchange-admin-center"></a>نهج الاستبقاء في مركز أداره Exchange

إذا كنت تريد ان نقوم بتشغيل التدقيق التلقائي للإعدادات المذكورة أدناه ، فحدد الزر السابق <--في اعلي هذه الصفحة ، ثم ادخل عنوان البريد الكتروني الخاص بالمستخدم الذي لديه مشاكل في نهج الاستبقاء.

 **المشكلة:** لا يتم تطبيق نهج الاستبقاء التي تم إنشاؤها أو تحديثها حديثا في "مركز أداره Exchange" علي علب البريد أو العناصر التي لا يتم نقلها إلى علبه بريد الأرشيف أو حذفها. 
  
 **الأسباب الاساسيه:**
  
- قد يعود سبب ذلك إلى عدم قيام **مساعد المجلد المدار** بمعالجه علبه بريد المستخدم. يحاول مساعد المجلد المدار معالجه كل علبه بريد في المؤسسة المستندة إلى السحابة مره واحده كل سبعه أيام. إذا قمت بتغيير علامة استبقاء أو تطبيق نهج استبقاء مختلف علي علبه بريد ، فيمكنك الانتظار حتى يقوم المجلد المدار بمعالجه علبه البريد ، أو يمكنك تشغيل الأمر ماناجيدفولديراسيستانت cmdlet لبدء تشغيل "مساعد المجلد المدار" لمعالجه علبه بريد معينه. يعتبر تشغيل أمر cmdlet هذا مفيدا لاختبار إعدادات نهج الاستبقاء أو علامة الاستبقاء أو استكشاف الأخطاء فيها. لمزيد من المعلومات ، قم بزيارة [تشغيل مساعد المجلد المدار](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **الحل:** قم بتشغيل الأمر التالي لبدء تشغيل مساعد المجلد المدار لعلبه بريد معينه:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- قد يحدث هذا أيضا إذا تم **تمكين** **ريتينتيونهولد** علي علبه البريد. إذا تم وضع علبه البريد علي ريتينتيونهولد ، فلن تتم معالجه نهج الاستبقاء علي علبه البريد خلال هذا الوقت. للحصول علي مزيد من الإينفورماتون علي اعداد ريتينتيونهولد ، راجع: [احتجاز استبقاء علبه البريد](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Solution**
    
  - تحقق من حاله اعداد ريتينتيونهولد علي علبه البريد المحددة في [أكسو powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - قم بتشغيل الأمر التالي **لتعطيل** ريتينتيونهولد علي علبه بريد معينه:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - الآن ، أعد تشغيل مساعد المجلدات المدارة:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **ملاحظه:** إذا كانت علبه البريد أصغر من 10 ميغابايت ، فلن يعالج مساعد المجلد المدار علبه البريد تلقائيا.
 
للحصول علي مزيد من المعلومات حول نهج الاستبقاء في مركز أداره Exchange ، راجع:
- [علامات الاستبقاء ونهج الاستبقاء](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [تطبيق نهج استبقاء علي علب البريد](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [أضافه علامات الاستبقاء أو ازالتها](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [كيفيه تحديد نوع التعليق الموضوع علي علبه بريد](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
