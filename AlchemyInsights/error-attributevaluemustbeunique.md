---
title: أتريبوتيفالويموستبيونيك الخطا
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
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709138"
---
# <a name="error-attributevaluemustbeunique"></a>الخطا: أتريبوتيفالويموستبيونيك

السبب الأكثر شيوعا للخطا أتريبوتيفالويموستبيونيك هو كائنين بسورسيانتشور مختلفتين (إيموتابليد) لديهما نفس القيمة للسمات ProxyAddresses و/أو القيم الاساسيه. لإصلاح الخطا أتريبوتيفالويموستبيونيك:
  
1. تعرف علي الproxyAddresses المكررة أو قيمه السمة الأخرى التي تتسبب في حدوث الخطا. يمكنك أيضا تحديد الكائنين (أو أكثر) المضمنين في التعارض. يمكن للتقرير الذي تم إنشاؤه بواسطة الحماية في Azure AD Connect للمزامنة مساعدتك في تحديد الكائنين.
    
2. تحديد العنصر الذي يجب ان يستمر في الحصول علي القيمة المكررة والعنصر الذي لا يجب ان يكون كذلك.
    
3. قم بازاله القيمة المكررة من العنصر الذي لا يجب ان تحتوي علي هذه القيمة. لاحظ انه يجب القيام بالتغيير في الدليل الذي تم فيه المصدر من قبل الكائن. في بعض الحالات ، قد تحتاج إلى حذف أحد العناصر المتعارضة.
    
4. إذا قمت بالتغيير في الإعلانات المحلية ، فيمكنك السماح ل Azure AD Connect بمزامنة التغيير الذي حدث فيه الخطا لكي يتم إصلاحه.
    

