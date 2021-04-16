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
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813747"
---
# <a name="error-attributevaluemustbeunique"></a>خطأ: AttributeValueMustBeUnique

السبب الأكثر شيوعا للخطأ AttributeValueMustBeUnique هو وجود كائنات مختلفة SourceAnchor (immutableId) لها القيمة نفسها لقيمة ProxyAddresses و/أو UserPrincipalName. لإصلاح الخطأ AttributeValueMustBeUnique:
  
1. تحديد proxyAddresses أو userPrincipalName أو قيمة سمة أخرى مكررة تتسبب في حدوث الخطأ. تعرف أيضا على أي من الكائنات (أو أكثر) المشاركين في التعارض. يمكن أن يساعدك التقرير الذي تم إنشاؤه بواسطة Azure AD Connect Health للمزامنة في تحديد هذين الأمرين.
    
2. تحديد الكائن الذي يجب أن يستمر في الحصول على القيمة المكررة وما هو الكائن الذي يجب ألا يكون مكررا.
    
3. قم بإزالة القيمة المكررة من الكائن الذي يجب ألا يكون له هذه القيمة. تجدر الإشارة إلى أنه يجب إجراء التغيير في الدليل الذي تم مصدر الكائن منه. في بعض الحالات، قد تحتاج إلى حذف أحد العناصر المتضاربة.
    
4. إذا قمت بالتغيير في AD في الموقع، فدع Azure AD Connect يتزامن التغيير للحصول على تصحيح للخطأ.
    

