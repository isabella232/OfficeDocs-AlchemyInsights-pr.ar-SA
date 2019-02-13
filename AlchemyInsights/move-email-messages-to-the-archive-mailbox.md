---
title: نقل رسائل البريد الإلكتروني إلى أرشيف علبة البريد
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a631af20e28a531a40f078e290239a372c38ab74
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29941684"
---
مشاكل أرشفة العناصر إلى أرشيف علبة البريد. تأكد من قيامك بتنفيذ الخطوات التالية:
  
1. تأكد من أن **أرشفة علبة البريد** تم تمكينه. إذا لم يكن الأمر كذلك، استخدم الخطوات في [هذه المقالة](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) لتمكين علبة البريد الأرشيف. 
    
2. في مركز مسؤول Exchange، حدد **علامات الاستبقاء** تحت **إدارة التوافق**، إنشاء **علامة استبقاء** مع عمل **نقل أرشيف** يتضمن المطلوب **الاستبقاء**.
    
3. في مركز مسؤول Exchange، حدد **نهج الاستبقاء**وإنشاء **نهج الاستبقاء** وإضافة علامة استبقاء **نقل أرشيف** لذلك النهج. 
    
4. [تعيين "نهج الاستبقاء"](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) لعلبة البريد لمستخدم معين. سيتم تطبيق نفس النهج **الأساسي** و **أرشيف** علبة البريد. 
    
علبة بريد المستخدم يجب الآن نهج أرشيف لنقل العناصر إلى أرشيف علبة البريد. قد يكون من الضروري فرض إدارة مجلد مساعد (وزارة الخارجية) لتشغيل وتطبيق الإعدادات الجديدة بعلبة بريد مستخدم. تشغيل الأمر التالي أثناء [الاتصال ب PowerShell أكسو](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) لبدء إدارة "مساعد المجلدات" لعلبة بريد محددة: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

للمزيد من المعلومات حول إعداد نهج أرشيف، راجع [إعداد نهج الأرشيف والحذف لعلب البريد](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

