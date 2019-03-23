---
title: أتريبوتيفالويموستبيونيك خطأ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7fc1190fb7b93dce945e366cf8b90112a97a2f3f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/22/2019
ms.locfileid: "30766011"
---
# <a name="error-attributevaluemustbeunique"></a>خطأ: أتريبوتيفالويموستبيونيك

السبب الأكثر شيوعاً للأخطاء أتريبوتيفالويموستبيونيك كائنين مع مختلف سورسينتشور (إيموتابليد) يحتوي على نفس القيمة للسمات ProxyAddresses و/أو UserPrincipalName. لتصحيح الخطأ أتريبوتيفالويموستبيونيك:
  
1. تحديد proxyAddresses المكررة أو userPrincipalName أو قيمة سمة أخرى تسبب هذا الخطأ. تحديد الكائنات (أو أكثر) التي تشارك في الصراع. تقرير أنشأها Azure الإعلان "الاتصال الصحة" للمزامنة يمكن أن يساعدك في تحديد الكائنين.
    
2. تحديد الكائن الذي ينبغي أن يكون القيمة المكررة والكائن الذي يجب أن لا.
    
3. إزالة القيمة المكررة من الكائن الذي يجب أن لا تحتوي على هذه القيمة. لاحظ أنه يجب إجراء التغيير في الدليل حيث مصدرها الكائن. في بعض الحالات، قد تحتاج إلى حذف أحد الكائنات في الصراع.
    
4. إذا قمت بالتغيير في أماكن العمل في الإعلان، تتيح مزامنة التغيير للخطأ للحصول على إصلاح الاتصال الإعلان Azure.
    

