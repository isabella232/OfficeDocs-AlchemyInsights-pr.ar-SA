---
title: التحقق من مجالك
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770978"
---
# <a name="verify-your-domain"></a>التحقق من مجالك

 **على الأرجح لم يتم تحديث السجل عبر الإنترنت.**
  
يستغرق الأمر عادة بضع دقائق لكي نتمكن من رؤية السجل الجديد، ولكن قد يستغرق ذلك أحيانا بضع ساعات. 
  
- إذا انتظرت هذه المدة، فتحقق مرة أخرى من أنك نسخت القيمة الدقيقة ولصقتها في سجل التحقق من صحة TXT لدى مضيف DNS. إحدى المشاكل الشائعة هي عدم بما في ذلك الجزء "MS=" من السجل. نحتاج إلى ذلك أيضا!

- في بعض مضيفي DNS، يجب عليك اتخاذ خطوة إضافية لحفظ ملف المنطقة (حيث يتم تخزين سجل DNS) بحيث يتم تحديثه عبر الإنترنت. تأكد من حفظ التغييرات حتى تتمكن Microsoft من رؤية السجل والتحقق منه.
