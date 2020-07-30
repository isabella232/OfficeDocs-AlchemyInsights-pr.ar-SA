---
title: نُهج الاستبقاء في مركز إدارة Exchange لا تعمل
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
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522794"
---
# <a name="retention-policies-in-exchange-admin-center"></a>نُهج الاستبقاء في مركز إدارة Exchange

إذا كنت تريد منا تشغيل الشيكات التلقائية للإعدادات المذكورة أدناه، حدد زر العودة <-- في أعلى هذه الصفحة، ثم أدخل عنوان البريد الإلكتروني للمستخدم الذي لديه مشاكل مع سياسات الاستبقاء.

 **المسألة:** نُهج الاستبقاء التي تم إنشاؤها حديثاً أو تحديثها في مركز إدارة Exchange لا يتم تطبيقها على علب البريد أو لا يتم نقل العناصر إلى علبة بريد الأرشيف أو حذفها. 
  
 **الأسباب الجذرية:**
  
- قد يكون هذا بسبب **"مساعد المجلد المدار"** لم تتم معالجة علبة البريد الخاصة بالمستخدم. يحاول "مساعد المجلد المُدار" معالجة كل علبة بريد في المؤسسة المستندة إلى مجموعة النظراء مرة كل سبعة أيام. إذا قمت بتغيير علامة استبقاء أو تطبيق نهج استبقاء مختلف على علبة بريد، يمكنك الانتظار حتى معالجة "مساعدة المجلدات المدارة" علبة البريد، أو يمكنك تشغيل cmdlet Start-ManagedFolderAssistant لبدء "مساعد المجلدات المدارة" لمعالجة علبة بريد معينة. إن تشغيل cmdlet هذا مفيد لاختبار أو استكشاف نهج استبقاء أو إعدادات علامة الاستبقاء وإصلاحها. لمزيد من المعلومات، قم بزيارة [تشغيل مساعد المجلدات المدارة](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **الحل:** تشغيل الأمر التالي لبدء تشغيل "مساعد المجلدات المدارة" لعلبة بريد معينة:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- قد يحدث هذا أيضًا إذا تم **تمكين** **استبقاء** على علبة البريد. إذا تم وضع علبة البريد على استبقاء، لن تتم معالجة نهج الاستبقاء على علبة البريد خلال ذلك الوقت. لمزيد من المعلومات على إعداد الاحتفاظ انظر: [احتجاز الاحتفاظ علبة البريد](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **حل:**
    
  - تحقق من حالة إعداد الاحتفاظ على علبة البريد المحددة في [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - تشغيل الأمر التالي **لتعطيل** الاحتفاظ على علبة بريد معينة:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - الآن، إعادة تشغيل "مساعد المجلد المدارة":
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **ملاحظة:** إذا كان علبة بريد أصغر من 10 ميغابايت، مساعد المجلدات المدارة لا تلقائياً معالجة علبة البريد.
 
لمزيد من المعلومات حول نُهج الاستبقاء في مركز إدارة Exchange، راجع:
- [علامات الاستبقاء وسياسات الاستبقاء](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [تطبيق نهج استبقاء على علب البريد](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [إضافة علامات الاستبقاء أو إزالتها](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [كيفية تحديد نوع احتجاز وضع على علبة بريد](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
