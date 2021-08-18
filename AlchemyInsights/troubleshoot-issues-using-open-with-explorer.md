---
title: استكشاف الأخطاء وإصلاحها باستخدام "فتح باستخدام المستكشف"
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 49d6d449af6e718d70c9948a03f7e2e1e21517d2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323553"
---
# <a name="fix-problems-with-open-with-explorer"></a>إصلاح المشاكل المتعلقة بالفتح باستخدام المستكشف

إصلاح المشاكل الشائعة عند فتح مكتبة مستندات في SharePoint أو OneDrive باستخدام الأمر **فتح بواسطة المستكشف:** 
  
- استخدم Internet Explorer 10 Internet Explorer 11. **لا يتوافق الفتح** مع المستكشف مع Microsoft Edge و Google Chrome و Firefox و الآخرين. **يتم تعطيل "فتح** باستخدام المستكشف" في كل المستعرضات باستثناء Internet Explorer. 
    
- **فتح باستخدام المستكشف** غير متوفر في التجربة الحديثة SharePoint مكتبات. استخدم **طريقة العرض في مستكشف الملفات** بدلا من ذلك. حدد **خيارات العرض** عرض في \> **مستكشف الملفات**. لا تتوافق طريقة العرض في "مستكشف الملفات" مع Microsoft Edge و Google Chrome و Firefox و غيرها. **عرض في مستكشف الملفات** المتوفر فقط في Internet Explorer. 
    
- تأكد من تشغيل خدمة WebClient. في مربع Windows البحث، اكتب تشغيل، وحدد تشغيل تطبيق سطح المكتب، وا اكتب services.msc، ثم اضغط على Enter. قم بالتمرير لأسفل وصولا إلى خدمة  WebClient وتأكد من عرض عمود الحالة "قيد التشغيل". إذا لم يحدث ذلك، انقر نقرا مزدوجا فوق الخدمة، وانقر **فوق** بدء ، ثم انقر فوق **موافق**. (قد تحتاج أولا إلى تمكين الخدمة  عن طريق تحديد يدوي أو تلقائي **في** المربع **نوع بدء** التشغيل.) 
    
**ملاحظة:** إن فتح مكتبة في "مستكشف الملفات" مفيد إذا كنت بحاجة إلى نسخ ملفات ومجلدات متعددة أو نقلها مرة واحدة، ولكن إذا كنت تريد العمل بشكل منتظم في المكتبة، نوصي بمزامنتها. لاستكشف المشاكل التي يتم فتحها في مستكشف الملفات وإصلاحها، راجع [فتح في المستكشف](https://go.microsoft.com/fwlink/?linkid=871665). للحصول على معلومات حول إعداد المزامنة، راجع [SharePoint الملفات باستخدام عميل المزامنة من OneDrive الجديد.](https://go.microsoft.com/fwlink/?linkid=871666)
  
الرجاء الاطلاع على المقالة كيفية استخدام الأمر "فتح باستخدام [المستكشف"](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) لاستكشف المشاكل وإصلاحها في SharePoint Online للحصول على مزيد من المعلومات. 
  

