---
title: استكشاف الأخطاء وإصلاحها باستخدام "فتح بواسطة المستعرض"
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
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659045"
---
# <a name="fix-problems-with-open-with-explorer"></a>إصلاح المشاكل المتعلقة بالفتح باستخدام المستكشف

إصلاح المشاكل الشائعة في فتح مكتبه مستندات في SharePoint أو OneDrive باستخدام الأمر **فتح بواسطة المستعرض** : 
  
- استخدم Internet Explorer 10 أو Internet Explorer 11. **الفتح باستخدام المستكشف** غير متوافق مع Microsoft Edge و Google Chrome و Firefox وغيرها. **الفتح باستخدام المستكشف** معطل في كل المستعرضات باستثناء Internet Explorer. 
    
- لا يتوفر الخيار **فتح باستخدام المستكشف** في التجربة الحديثة لمكتبات SharePoint. استخدم **طريقه العرض في "مستكشف الملفات** " بدلا من ذلك. حدد طريقه عرض **خيارات** \> **العرض في "مستكشف الملفات**". طريقه العرض في "مستكشف الملفات" غير متوافقة مع Microsoft Edge و Google Chrome و Firefox وغيرها. تتوفر **طريقه العرض في "مستكشف الملفات** " في Internet explorer فقط. 
    
- تاكد من تشغيل خدمه WebClient. في مربع البحث في Windows ، اكتب تشغيل ، وحدد تشغيل تطبيق سطح المكتب ، واكتب services.msc ، ثم اضغط علي مفتاح الإدخال Enter. قم بالتمرير لأسفل وصولا إلى خدمه WebClient وتاكد من عرض عمود **الحالة** "قيد التشغيل". إذا لم يكن الأمر كذلك ، فانقر نقرا مزدوجا فوق الخدمة ، وانقر فوق **بدء**، ثم فوق **موافق**. (قد تحتاج إلى تمكين الخدمة أولا بتحديد اما **يدوي** أو **تلقائي** في المربع **نوع بدء التشغيل** .) 
    
> [!NOTE]
> يعد فتح مكتبه في "مستكشف الملفات" مفيدا إذا كنت بحاجه إلى نسخ ملفات ومجلدات متعددة أو نقلها مره واحده ، ولكن إذا كنت تريد العمل بشكل منتظم في المكتبة ، فنوصي بمزامنتها. لاستكشاف الأخطاء وإصلاحها في "مستكشف الملفات" ، راجع [فتح في "المستكشف"](https://go.microsoft.com/fwlink/?linkid=871665). للحصول علي معلومات حول اعداد المزامنة ، راجع [مزامنة ملفات SharePoint باستخدام عميل المزامنة من OneDrive الجديد](https://go.microsoft.com/fwlink/?linkid=871666).
  
الرجاء مراجعه المقالة [كيفيه استخدام الأمر "فتح بواسطة المستعرض" لاستكشاف الأخطاء وإصلاحها في SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) للحصول علي مزيد من المعلومات. 
  

