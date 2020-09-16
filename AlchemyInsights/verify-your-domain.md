---
title: التحقق من المجال
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734293"
---
# <a name="verify-your-domain"></a>التحقق من المجال

 **من المحتمل عدم تحديث السجل عبر الإنترنت.**
  
عاده ما يستغرق الأمر بضع دقائق فقط لكي يتمكنوا من رؤية السجل الجديد ، ولكن قد يستغرق الأمر بضع ساعات. 
  
- إذا قمت بالانتهاء من هذا الوقت بالفعل ، فتاكد من انك قمت بنسخ القيمة الصحيحة ولصقها في سجل التحقق من الصحة TXT لدي مضيف DNS. هناك مشكله واحده شائعه لا تتضمن الجزء "MS =" من السجل. نحتاج أيضا إلى ذلك!

- في بعض مضيفي DNS ، يجب اجراء خطوه اضافيه لحفظ ملف المنطقة (حيث يتم تخزين سجل DNS) بحيث يتم تحديثه عبر الإنترنت. تاكد من انك قمت بحفظ التغييرات التي أجريتها لكي تتمكن Microsoft من رؤية السجل والتحقق منه.
