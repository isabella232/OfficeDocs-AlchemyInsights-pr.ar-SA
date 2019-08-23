---
title: فتح باستخدام مستكشف لا يعمل
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538444"
---
# <a name="open-with-explorer-isnt-working"></a>فتح باستخدام مستكشف لا يعمل

إذا لم يعمل على **فتح باستخدام "مستكشف"** أو **طريقة عرض في "مستكشف الملفات"** تأكد من تعيين **تشغيل** خدمة WebClient باتباع الخطوات التالية. على سبيل المثال، قد يستغرق وقتاً طويلاً لفتح مكتبة SharePoint أو أندريف عند عدم تشغيل الخدمة. 
  
1. في مربع "البحث في Windows"، تشغيل نوع، حدد تطبيق سطح المكتب تشغيل ونوع services.msc ثم حدد **Enter**.
    
2. قم بالتمرير لأسفل إلى خدمة WebClient والتحقق من عمود **الحالة** . إذا حالة خدمة WebClient ليست **قيد التشغيل**، انقر نقراً مزدوجاً فوق الخدمة، انقر فوق **ابدأ**، وثم انقر فوق **موافق**. تمكين الخدمة، إذا لزم الأمر، عن طريق تحديد **يدوي** أو **تلقائي** في المربع **نوع بدء التشغيل** . 
    
> [!NOTE]
> استكشاف أخطاء مشاكل فتح "مستكشف الملفات"، راجع [فتح في مستكشف](https://go.microsoft.com/fwlink/?linkid=871665). استكشاف المزامنة كبديل أفضل: [الملفات SharePoint متزامنة مع عميل المزامنة أندريف الجديد](https://go.microsoft.com/fwlink/?linkid=871666). 
  

