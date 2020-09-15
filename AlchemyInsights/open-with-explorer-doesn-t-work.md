---
title: الفتح باستخدام المستكشف لا يعمل
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694443"
---
# <a name="open-with-explorer-isnt-working"></a>فتح باستخدام المستكشف لا يعمل

إذا كان الخيار **فتح باستخدام المستكشف** أو **العرض في "مستكشف الملفات"** لا يعمل ، فتاكد من انه قد تم تعيين خدمه WebClient **ليتم تشغيلها** من خلال اتباع الخطوات أدناه. علي سبيل المثال ، قد يستغرق فتح مكتبه SharePoint أو OneDrive وقتا طويلا عندما لا تكون الخدمة قيد التشغيل. 
  
1. في مربع البحث في Windows ، اكتب تشغيل ، وحدد تشغيل تطبيق سطح المكتب ، واكتب services.msc ، ثم حدد **Enter**.
    
2. قم بالتمرير لأسفل وصولا إلى خدمه WebClient وتحقق من عمود **الحالة** . إذا لم تكن حاله خدمه WebClient **قيد التشغيل**، فانقر نقرا مزدوجا فوق الخدمة ، وانقر فوق **بدء**، ثم فوق **موافق**. تمكين الخدمة ، إذا لزم الاجراء ، بتحديد اما **يدوي** أو **تلقائي** في المربع **نوع بدء التشغيل** . 
    
> [!NOTE]
> لاستكشاف الأخطاء وإصلاحها في "مستكشف الملفات" ، راجع [فتح في "المستكشف"](https://go.microsoft.com/fwlink/?linkid=871665). استكشاف المزامنة كبديل أفضل: [مزامنة ملفات SharePoint باستخدام عميل المزامنة من OneDrive الجديد](https://go.microsoft.com/fwlink/?linkid=871666). 
  

