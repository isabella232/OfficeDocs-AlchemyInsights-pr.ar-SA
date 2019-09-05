---
title: استكشاف المشكلات وإصلاحها باستخدام فتح باستخدام Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742720"
---
# <a name="fix-problems-with-open-with-explorer"></a>إصلاح المشاكل مع فتح مع مستكشف

إصلاح المشكلات الشائعة حول فتح مكتبة مستندات في SharePoint أو أندريف باستخدام الأمر **فتح باستخدام** مستكشف: 
  
- استخدام Internet Explorer 10 أو Internet Explorer 11. **فتح مع إكسبلورر** غير متوافق مع مايكروسوفت إيدج، جوجل كروم، فايرفوكس وغيرها. **فتح مع مستكشف** مع تعطيل في كافة المستعرضات باستثناء Internet Explorer. 
    
- **فتح مع مستكشف** غير متوفر في التجربة الحديثة لمكتبات SharePoint. استخدام **طريقة العرض في "مستكشف الملفات"** بدلاً من ذلك. حدد **عرض خيارات** \> **العرض في مستكشف الملفات**. عرض في مستكشف الملفات غير متوافق مع مايكروسوفت إيدج، جوجل كروم، فايرفوكس وغيرها. **عرض في مستكشف الملفات** في متوفر فقط في Internet Explorer. 
    
- تأكد من تشغيل خدمة WebClient. في مربع البحث في Windows، اكتب تشغيل، حدد تشغيل تطبيق سطح المكتب، اكتب services.msc، ثم اضغط Enter. قم بالتمرير لأسفل إلى خدمة WebClient وتأكد من عرض عمود **الحالة** "قيد التشغيل". إذا لم يكن كذلك، انقر نقراً مزدوجاً فوق الخدمة، وانقر فوق **ابدأ**، ثم انقر فوق **موافق**. (قد تحتاج أولاً إلى تمكين الخدمة عن طريق تحديد **إما يدوي** أو **تلقائي** في المربع نوع **بدء التشغيل.)** 
    
> [!NOTE]
> فتح مكتبة في مستكشف الملفات مفيد إذا كنت بحاجة إلى نسخ أو نقل ملفات ومجلدات متعددة مرة واحدة، ولكن إذا كنت ترغب في العمل بانتظام في المكتبة، نوصي بمزامنتها. لاستكشاف المشكلات التي يتم فتحها في مستكشف الملفات وإصلاحها، راجع [فتح في Explorer](https://go.microsoft.com/fwlink/?linkid=871665). للحصول على معلومات حول إعداد المزامنة، راجع [مزامنة ملفات SharePoint مع عميل المزامنة OneDrive الجديد](https://go.microsoft.com/fwlink/?linkid=871666).
  
الرجاء مراجعة المقالة [كيفية استخدام الأمر "فتح باستخدام مستكشف" لاستكشاف المشكلات في SharePoint على الإنترنت](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) للحصول على مزيد من المعلومات. 
  

