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
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526954"
---
# <a name="error-attributevaluemustbeunique"></a>خطأ: أتريبوتيفالويموستبيونيك

السبب الأكثر شيوعاً للأخطاء أتريبوتيفالويموستبيونيك كائنين مع مختلف سورسينتشور (إيموتابليد) يحتوي على نفس القيمة للسمات ProxyAddresses و/أو UserPrincipalName. لتصحيح الخطأ أتريبوتيفالويموستبيونيك:
  
1. تحديد proxyAddresses المكررة أو userPrincipalName أو قيمة سمة أخرى تسبب هذا الخطأ. تحديد الكائنات (أو أكثر) التي تشارك في الصراع. تقرير أنشأها Azure الإعلان "الاتصال الصحة" للمزامنة يمكن أن يساعدك في تحديد الكائنين.
    
2. تحديد الكائن الذي ينبغي أن يكون القيمة المكررة والكائن الذي يجب أن لا.
    
3. إزالة القيمة المكررة من الكائن الذي يجب أن لا تحتوي على هذه القيمة. لاحظ أنه يجب إجراء التغيير في الدليل حيث مصدرها الكائن. في بعض الحالات، قد تحتاج إلى حذف أحد الكائنات في الصراع.
    
4. إذا قمت بالتغيير في أماكن العمل في الإعلان، تتيح مزامنة التغيير للخطأ للحصول على إصلاح الاتصال الإعلان Azure.
    

