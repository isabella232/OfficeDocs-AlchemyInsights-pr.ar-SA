---
title: استكشاف أخطاء وإصلاحها باستخدام فتح باستخدام مستكشف
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: c95f07b9fb7251442577c014e4005dbe3f92ceb4
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661738"
---
# <a name="fix-problems-with-open-with-explorer"></a>إصلاح المشاكل المتعلقة بفتح باستخدام مستكشف

إصلاح المشاكل الشائعة المتعلقة بفتح مكتبة مستندات SharePoint أو أندريف باستخدام الأمر **فتح بواسطة المستعرض** : 
  
- استخدام Internet Explorer 10 أو 11 من برنامج Internet Explorer. **فتح باستخدام مستكشف** غير متوافق مع Microsoft الحافة، جوجل كروم، فايرفوكس وغيرها. **فتح باستخدام "مستكشف"** معطل في كافة المستعرضات استثناء Internet Explorer. 
    
- **فتح باستخدام "مستكشف"** غير متوفر في التجربة الحديثة لمكتبات SharePoint. استخدم **طريقة عرض في "مستكشف الملفات"** بدلاً من ذلك. حدد **خيارات العرض** \> **طريقة عرض في "مستكشف الملفات"**. طريقة عرض في "مستكشف الملفات" غير متوافق مع Microsoft الحافة، جوجل كروم، فايرفوكس وغيرها. **طريقة عرض في "مستكشف الملفات"** في متوفر فقط في Internet Explorer. 
    
- تأكد من تشغيل خدمة WebClient. في المربع بحث Windows، نوع التشغيل، حدد سطح المكتب تشغيل التطبيق ثم اكتب services.msc وثم اضغط Enter. قم بالتمرير لأسفل إلى خدمة WebClient وتأكد من أن يعرض عمود **الحالة** "قيد التشغيل". إذا لم يكن كذلك، انقر نقراً مزدوجاً فوق الخدمة، انقر فوق **ابدأ**، وثم انقر فوق **موافق**. (قد تحتاج إلى تمكين الخدمة أولاً بتحديد أما **يدوياً** أو **تلقائياً** في المربع **نوع بدء التشغيل** ). 
    
> [!NOTE]
> فتح مكتبة في "مستكشف الملفات" مفيد إذا كنت تريد نسخ أو نقل ملفات ومجلدات متعددة مرة واحدة، ولكن إذا كنت تريد أن تعمل بشكل منتظم في المكتبة، نوصي بمزامنته. استكشاف أخطاء مشاكل فتح "مستكشف الملفات"، راجع [فتح في مستكشف](https://go.microsoft.com/fwlink/?linkid=871665). للحصول على مزيد من المعلومات حول إعداد المزامنة، راجع [الملفات SharePoint متزامنة مع عميل المزامنة أندريف الجديد](https://go.microsoft.com/fwlink/?linkid=871666).
  
الرجاء مراجعة المقالة [كيفية استخدام الأمر "فتح باستخدام" مستكشف "" لاستكشاف مشاكل في SharePoint عبر إنترنت](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) للحصول على مزيد من المعلومات. 
  

