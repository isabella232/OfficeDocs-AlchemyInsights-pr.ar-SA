---
title: لا يعمل "فتح باستخدام المستكشف"
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
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321848"
---
# <a name="open-with-explorer-isnt-working"></a>لا يعمل "فتح باستخدام المستكشف"

إذا لم يعمل فتح **بواسطة المستكشف** أو طريقة العرض في **مستكشف** الملفات، فتأكد من تعيين خدمة WebClient إلى **تشغيل** باتباع الخطوات أدناه. على سبيل المثال، قد يستغرق فتح مكتبة SharePoint أو OneDrive وقت لا تكون فيه الخدمة قيد التشغيل. 
  
1. في مربع Windows البحث، اكتب تشغيل، وحدد تشغيل تطبيق سطح المكتب، وا اكتب services.msc، ثم حدد **Enter**.
    
2. قم بالتمرير لأسفل وصولا إلى خدمة WebClient وتحقق من **عمود** الحالة. إذا لم تكن حالة خدمة WebClient قيد التشغيل، **انقر** نقرا مزدوجا فوق الخدمة، وانقر **فوق** بدء ، ثم انقر فوق **موافق**. قم بتمكين الخدمة، إذا لزم  الأمر، عن طريق تحديد يدوي أو تلقائي **في** المربع **نوع بدء** التشغيل. 
    
**ملاحظة:** لاستكشف المشاكل التي يتم فتحها في مستكشف الملفات وإصلاحها، راجع [فتح في المستكشف](https://go.microsoft.com/fwlink/?linkid=871665). استكشاف المزامنة كبديل أفضل: [SharePoint الملفات باستخدام المزامنة من OneDrive الجديد.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

