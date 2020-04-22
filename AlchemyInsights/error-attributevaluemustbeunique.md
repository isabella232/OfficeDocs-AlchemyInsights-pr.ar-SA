---
title: خطأ AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703161"
---
# <a name="error-attributevaluemustbeunique"></a>خطأ: AttributeValueMustBeUnique

السبب الأكثر شيوعاً للخطأ AttributeValueMustBeUnique هو كائنين مع SourceAnchor مختلفة (immutableId) لها نفس القيمة لخصائص ProxyAddresses و /أو UserPrincipalName. لإصلاح خطأ AttributeValueMustBeUnique:
  
1. تحديد عنوان الوكيل المكرر أو userPrincipalName أو قيمة السمة الأخرى التي تسبب الخطأ. حدد أيضًا أي كائنين (أو أكثر) متورطين في التعارض. يمكن أن يساعدك التقرير الذي تم إنشاؤه بواسطة Azure AD Connect Health للمزامنة في التعرف على الكائنين.
    
2. تحديد الكائن الذي يجب أن يستمر في الحصول على القيمة المكررة والكائن الذي لا يجب.
    
3. إزالة القيمة المكررة من الكائن الذي يجب أن لا يكون هذه القيمة. لاحظ أنه يجب إجراء التغيير في الدليل حيث يتم الحصول على الكائن من. في بعض الحالات، قد تحتاج إلى حذف أحد الكائنات في تعارض.
    
4. إذا قمت بالتغيير في الإعلان في أماكن العمل، فدع Azure AD Connect يقوم بمزامنة التغيير حتى يتم إصلاح الخطأ.
    

