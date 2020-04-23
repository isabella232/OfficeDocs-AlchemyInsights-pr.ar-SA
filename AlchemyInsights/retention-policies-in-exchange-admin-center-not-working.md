---
title: سياسات الاحتفاظ في مركز إدارة Exchange لا تعمل
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742420"
---
# <a name="retention-policies-in-exchange-admin-center"></a>سياسات الاحتفاظ في مركز إدارة Exchange

 **المشكلة:** لا يتم تطبيق نُهج الاحتفاظ التي تم إنشاؤها أو تحديثها حديثًا في مركز Exchange Admin على صناديق البريد أو العناصر التي لا يتم نقلها إلى صندوق بريد الأرشيف أو حذفها. 
  
 **الأسباب الجذرية:**
  
- قد يكون هذا بسبب لم يعالج **"مساعد المجلد المدار"** علبة بريد المستخدم. يحاول "مساعد المجلد المدار" معالجة كل علبة بريد في المؤسسة المستندة إلى مجموعة النظراء مرة كل سبعة أيام. إذا قمت بتغيير علامة الاحتفاظ أو تطبيق نهج استبقاء مختلف على علبة بريد، يمكنك الانتظار حتى يعالج "مساعدة المجلد المدارة" علبة البريد، أو يمكنك تشغيل cmdlet بدء التشغيل المدارة FolderAssistant لبدء تشغيل "مساعد المجلد المدارة" لمعالجة علبة بريد معينة. تشغيل هذا cmdlet مفيد لاختبار أو استكشاف الأخطاء وإصلاحها نهج الاحتفاظ أو إعدادات علامة الاحتفاظ. لمزيد من المعلومات، قم [بزيارة تشغيل مساعد المجلد المدار](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **الحل:** تشغيل الأمر التالي لبدء تشغيل "مساعد المجلد المدارة" لعلبة بريد معينة:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- قد يحدث هذا أيضاً إذا تم **تمكين** **RetentionHold** على علبة البريد. إذا تم وضع علبة البريد على HoldHold، لن تتم معالجة نهج الاحتفاظ على علبة البريد خلال ذلك الوقت. لمزيد من المعلوماتية على إعداد RetentionHold انظر: [احتجاز الاحتفاظ بعلبة البريد](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **حل:**
    
  - تحقق من حالة إعداد RetentionHold على علبة بريد محددة في [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - تشغيل الأمر التالي **لتعطيل** RetentionHoldعلى علبة بريد معينة:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - الآن، إعادة تشغيل "مساعد المجلد المدارة":
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **ملاحظة:** إذا كان علبة البريد أصغر من 10 ميغابايت، لن يقوم "مساعد المجلد المدار" بمعالجة علبة البريد تلقائياً.
 
لمزيد من المعلومات حول نُهج الاحتفاظ في مركز إدارة Exchange، راجع:
- [علامات الاحتفاظ وسياسات الاحتفاظ](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [تطبيق نهج الاحتفاظ على علب البريد](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [إضافة علامات الاحتفاظ أو إزالتها](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [كيفية تحديد نوع الانتظار الموضوع على علبة بريد](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
