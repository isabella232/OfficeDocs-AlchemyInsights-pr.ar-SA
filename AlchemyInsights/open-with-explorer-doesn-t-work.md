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
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: f788c3c626cdeb19970edb59563c59eea60e2992
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906791"
---
# <a name="open-with-explorer-isnt-working"></a>فتح باستخدام مستكشف لا يعمل

إذا لم يعمل على **فتح باستخدام "مستكشف"** أو **طريقة عرض في "مستكشف الملفات"** تأكد من تعيين **تشغيل** خدمة WebClient باتباع الخطوات التالية. على سبيل المثال، قد يستغرق وقتاً طويلاً لفتح مكتبة SharePoint أو أندريف عند عدم تشغيل الخدمة. 
  
1. في مربع "البحث في Windows"، تشغيل نوع، حدد تطبيق سطح المكتب تشغيل ونوع services.msc ثم حدد **Enter**.
    
2. قم بالتمرير لأسفل إلى خدمة WebClient والتحقق من عمود **الحالة** . إذا حالة خدمة WebClient ليست **قيد التشغيل**، انقر نقراً مزدوجاً فوق الخدمة، انقر فوق **ابدأ**، وثم انقر فوق **موافق**. تمكين الخدمة، إذا لزم الأمر، عن طريق تحديد **يدوي** أو **تلقائي** في المربع **نوع بدء التشغيل** . 
    
> [!NOTE]
> استكشاف أخطاء مشاكل فتح "مستكشف الملفات"، راجع [فتح في مستكشف](https://go.microsoft.com/fwlink/?linkid=871665). استكشاف المزامنة كبديل أفضل: [الملفات SharePoint متزامنة مع عميل المزامنة أندريف الجديد](https://go.microsoft.com/fwlink/?linkid=871666). 
  

