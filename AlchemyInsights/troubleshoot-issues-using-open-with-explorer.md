---
title: استكشاف المشاكل وإصلاحها باستخدام فتح مع Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759679"
---
# <a name="fix-problems-with-open-with-explorer"></a>إصلاح المشاكل مع فتح مع مستكشف

إصلاح المشاكل الشائعة في فتح مكتبة مستندات في SharePoint أو OneDrive باستخدام الأمر **فتح مع Explorer:** 
  
- استخدم إنترنت إكسبلورر 10 أو إنترنت إكسبلورر 11. **فتح مع إكسبلورر** غير متوافق مع مايكروسوفت إيدج وجوجل كروم وفايرفوكس وغيرها. **تم** تعطيل فتح مع Explorer في جميع المتصفحات باستثناء Internet Explorer. 
    
- **فتح مع إكسبلورر** غير متوفر في التجربة الحديثة لمكتبات SharePoint. استخدم **طريقة العرض في مستكشف الملفات** بدلاً من ذلك. حدد **عرض خيارات** \> **العرض في مستكشف الملفات**. عرض في ملف إكسبلورر غير متوافق مع مايكروسوفت إيدج، جوجل كروم، فايرفوكس وغيرها. **عرض في مستكشف الملفات** في متوفر فقط في Internet Explorer. 
    
- تأكد من تشغيل خدمة WebClient. في مربع بحث Windows، اكتب التشغيل، وحدد تطبيق تشغيل سطح المكتب، واكتب services.msc، ثم اضغط على إدخال. مرر لأسفل إلى خدمة WebClient وتأكد من عرض عمود **الحالة** "قيد التشغيل". إذا لم يكن كذلك، انقر نقراً مزدوجاً على الخدمة، انقر فوق **ابدأ،** ثم انقر فوق **موافق**. (قد تحتاج أولاً إلى تمكين الخدمة عن طريق تحديد **إما يدوي** أو **تلقائي** في مربع نوع **بدء التشغيل.)** 
    
> [!NOTE]
> يعد فتح مكتبة في File Explorer مفيدًا إذا كنت بحاجة إلى نسخ ملفات ومجلدات متعددة أو نقلها مرة واحدة ، ولكن إذا كنت ترغب في العمل بانتظام في المكتبة ، فإننا نوصي بمزامنتها. لاستكشاف المشاكل التي يتم فتحها في مستكشف الملفات، راجع [فتح في Explorer](https://go.microsoft.com/fwlink/?linkid=871665). للحصول على معلومات حول إعداد المزامنة، راجع [ملفات مزامنة SharePoint مع عميل مزامنة OneDrive الجديد](https://go.microsoft.com/fwlink/?linkid=871666).
  
الرجاء الاطلاع على المقالة [كيفية استخدام الأمر "فتح مع مستكشف" لاستكشاف المشكلات في SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) لمزيد من المعلومات. 
  

