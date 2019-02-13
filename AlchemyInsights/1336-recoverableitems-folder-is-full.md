---
title: 1336 ريكوفيرابليتيمس المجلد ممتلئ
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: dbf4930c34e4175a14b77fab4eafc953bb37cc02
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29909275"
---
# <a name="the-recoverable-items-folder-is-full"></a>امتلاء المجلد "العناصر القابلة للاسترداد"

علب بريد Exchange عبر الإنترنت في Office 365، حد التخزين الافتراضي للمجلد "العناصر القابلة للاسترداد" بالنسبة سعة 30 جيجابايت. حد التخزين للمجلد "العناصر القابلة للاسترداد" تلقائياً تزداد إلى 100 جيجابايت حالة علبة البريد على "إجراء التقاضي"، اضغط eDiscovery، أو يتم تعيين نهج استبقاء Office 365.
  
عندما يصل المجلد "العناصر القابلة للاسترداد" إلى حد التخزين، تتأثر وظيفة علبة البريد بالطرق التالية:
  
- يتعذر على المستخدم حذف العناصر من علبة البريد.
    
- لا يمكن حذف "مجلد مساعد المدار" العناصر استناداً إلى إعدادات المجلدات المدارة أو علامة استبقاء.
    
- علب البريد التي تمكين استرداد عنصر واحد أو وضعه قيد الإيقاف، لا الاحتفاظ بإصدارات العناصر التي يقوم المستخدم بتحرير عملية حماية الصفحة النسخ عند الكتابة.
    
- علب البريد التي تحتوي على علبة البريد تسجيل تمكين التدقيق، يمكن حفظ لم إدخالات سجل التدقيق علبة البريد في مجلد فرعي عمليات مراجعة الحسابات في مجلد "العناصر القابلة للاسترداد".
    
يمكن استخدام المسؤولين لصناديق البريد التي ليست قيد الاحتجاز، `Search-Mailbox -SearchDumpsterOnly -DeleteContent` في PowerShell Exchange عبر إنترنت حذف العناصر الموجودة في المجلد "العناصر القابلة للاسترداد". لمزيد من المعلومات، راجع المواضيع التالية: 
  
- [البحث عن الرسائل وحذفها](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [صندوق بريد البحث](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
علب البريد قيد الانتظار، يلزم المسؤولين إزالة الاحتجاز قبل أن يتمكنوا من العناصر المحذوفة من مجلد "العناصر القابلة للاسترداد". لمزيد من المعلومات، راجع [حذف العناصر الموجودة في المجلد من صناديق البريد المستندة إلى مجموعة النظراء على عقد "العناصر القابلة للاسترداد"](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).
  
زيادة حد التخزين من "العناصر القابلة للاسترداد" المجلد لعلب بريد على عقد وإعداد نهج استبقاء علبة بريد نقل العناصر من مجلد "العناصر القابلة للاسترداد" للأرشيف المستخدم للمساعدة في الحيلولة دون تحول كامل في مجلد "العناصر القابلة للاسترداد"، المسؤولين علبة البريد. راجع [زيادة الحصة النسبية لعلب بريد على عقد "العناصر القابلة للاسترداد"](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
  

