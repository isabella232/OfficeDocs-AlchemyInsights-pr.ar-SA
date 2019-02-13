---
title: نهج الاستبقاء في مركز مسؤول Exchange لا يعمل
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: c9061fa728edaab6575a7b1027783e56739a6d14
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934979"
---
# <a name="retention-policies-in-exchange-admin-center"></a>نهج الاستبقاء في مركز مسؤول Exchange

 **المشكلة:** المنشأة حديثا أو لا تطبق نهج الاستبقاء حدثت في مركز مسؤول Exchange إلى علب البريد أو عناصر نقل أرشيف علبة البريد أو حذفه لا. 
  
 **الأسباب الأساسية:**
  
- قد يرجع هذا **مساعد المجلد المدار** غير عالجت علبة بريد المستخدم. مساعد المجلد المدار يحاول معالجة كل علبة البريد في المؤسسة الخاصة بك إلى مجموعة النظراء مرة كل سبعة أيام. إذا غيرت علامة استبقاء أو تطبيق نهج استبقاء مختلفة لعلبة بريد، يمكنك الانتظار حتى "إدارة مجلد مساعدة" العمليات علبة البريد، أو يمكنك تشغيل الأمر cmdlet ماناجيدفولديراسيستانت ابدأ لبدء إدارة "مساعد المجلدات" لمعالجة معينة علبة البريد. تشغيل cmdlet هذا مفيداً لاستكشاف نهج استبقاء أو إعدادات علامة استبقاء أو الاختبار. لمزيد من المعلومات، قم بزيارة [تشغيل إدارة "مساعد المجلدات"](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **الحل:** قم بتشغيل الأمر التالي لتشغيل إدارة "مساعد المجلدات" لعلبة بريد محددة: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- هذا قد أيضا يحدث إذا تم **تمكين** على صندوق البريد **ريتينتيونهولد** . إذا تم وضع علبة البريد في ريتينتيونهولد، لن تتم معالجة نهج الاستبقاء في علبة البريد خلال تلك الفترة. لمعلومات أكثر راجع الإعداد ريتينتيونهولد: [اضغط الاحتفاظ بعلبة البريد](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **الحل:**
    
  - التحقق من حالة الإعداد ريتينتيونهولد في علبة بريد معينة في [أكسو powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - تشغيل الأمر التالي **تعطيل** ريتينتيونهولد على علبة بريد معينة: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - والآن، إعادة تشغيل مساعد المجلد المدارة:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **ملاحظة:** إذا كانت علبة بريد أصغر من 10 ميغابايت، "مساعد المجلد المدار" سوف لا تلقائياً معالجة علبة البريد. 
  

