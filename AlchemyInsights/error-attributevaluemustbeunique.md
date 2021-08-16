---
title: خطأ AttributeValueMustBeUnique
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
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002107"
---
# <a name="error-attributevaluemustbeunique"></a>خطأ: AttributeValueMustBeUnique

السبب الأكثر شيوعا للخطأ AttributeValueMustBeUnique هو وجود كائنات مختلفة SourceAnchor (immutableId) لها القيمة نفسها لقيمة ProxyAddresses و/أو UserPrincipalName. لإصلاح الخطأ AttributeValueMustBeUnique:
  
1. تحديد proxyAddresses أو userPrincipalName أو قيمة سمة أخرى مكررة تتسبب في حدوث الخطأ. تعرف أيضا على أي من الكائنات (أو أكثر) المشاركين في التعارض. يمكن أن يساعدك التقرير الذي تم إنشاؤه بواسطة Azure AD الاتصال "الصحة للمزامنة" على تحديد هذين الأمرين.
    
2. تحديد الكائن الذي يجب أن يستمر في الحصول على القيمة المكررة وما هو الكائن الذي يجب ألا يكون مكررا.
    
3. قم بإزالة القيمة المكررة من الكائن الذي يجب ألا يكون له هذه القيمة. تجدر الإشارة إلى أنه يجب إجراء التغيير في الدليل الذي تم مصدر الكائن منه. في بعض الحالات، قد تحتاج إلى حذف أحد العناصر المتضاربة.
    
4. إذا قمت بالتغيير في AD في الموقع، فدع Azure AD الاتصال التغيير للحصول على تصحيح للخطأ.
    

