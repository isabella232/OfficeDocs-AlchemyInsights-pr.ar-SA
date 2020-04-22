---
title: فتح مع مستكشف لا يعمل
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713021"
---
# <a name="open-with-explorer-isnt-working"></a>فتح مع مستكشف لا يعمل

إذا **كان فتح مع مستكشف** أو عرض في مستكشف **الملفات** لا يعمل تأكد من تعيين خدمة WebClient إلى **قيد التشغيل** باتباع الخطوات التالية. على سبيل المثال، قد يستغرق وقتاً طويلاً لفتح مكتبة SharePoint أو OneDrive عند عدم تشغيل الخدمة. 
  
1. في مربع بحث Windows، اكتب التشغيل، وحدد تطبيق تشغيل سطح المكتب، واكتب services.msc، ثم حدد **إدخال**.
    
2. مرر لأسفل إلى خدمة WebClient وتحقق من **عمود الحالة.** إذا لم تكن حالة خدمة WebClient **قيد التشغيل**، انقر نقرًا مزدوجًا على الخدمة ، انقر فوق **ابدأ**، ثم انقر فوق **موافق**. تمكين الخدمة، إذا لزم الأمر، عن طريق تحديد **إما يدوي** أو **تلقائي** في مربع نوع **بدء التشغيل.** 
    
> [!NOTE]
> لاستكشاف المشاكل التي يتم فتحها في مستكشف الملفات، راجع [فتح في Explorer](https://go.microsoft.com/fwlink/?linkid=871665). استكشاف المزامنة كبديل أفضل: [مزامنة ملفات SharePoint مع عميل مزامنة OneDrive الجديد](https://go.microsoft.com/fwlink/?linkid=871666). 
  

