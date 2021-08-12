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
ms.openlocfilehash: 9e258cfc70c57fe787830d659dc52f4696768bea164d3be9ce7bcb9e7123c5a9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971002"
---
# <a name="verify-your-domain"></a>التحقق من مجالك

 **على الأرجح لم يتم تحديث السجل عبر الإنترنت.**
  
يستغرق الأمر عادة بضع دقائق لكي نتمكن من رؤية السجل الجديد، ولكن قد يستغرق ذلك أحيانا بضع ساعات. 
  
- إذا انتظرت هذه المدة، فتحقق مرة أخرى من أنك نسخت القيمة الدقيقة ولصقتها في سجل التحقق من صحة TXT لدى مضيف DNS. إحدى المشاكل الشائعة هي عدم بما في ذلك الجزء "MS=" من السجل. نحتاج إلى ذلك أيضا!

- في بعض مضيفي DNS، يجب عليك اتخاذ خطوة إضافية لحفظ ملف المنطقة (حيث يتم تخزين سجل DNS) بحيث يتم تحديثه عبر الإنترنت. تأكد من حفظ التغييرات حتى تتمكن Microsoft من رؤية السجل والتحقق منه.
