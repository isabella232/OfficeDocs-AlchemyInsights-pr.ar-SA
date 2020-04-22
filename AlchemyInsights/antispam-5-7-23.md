---
title: مكافحة البريد المزعج - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676484"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>إصلاح مشكلات تسليم البريد الإلكتروني لرمز الخطأ 5.7.23

تحقق من سجل DNS SPF للمجال الخاص بك في مدقق سجل SPF أو DNS متوفر بشكل عام على الويب.

تحقق من أن الرسالة الصادرة لم يتم تعريفها كرسائل غير مرغوب فيها من قبل Microsoft وتم توجيهها من خلال [تجمع التسليم عالي الخطورة](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). لن تجتاز الرسائل الموجودة في تجمع التسليم عالي المخاطر شيكات SPF، وبالتالي لن يتم قبولها من قبل مؤسسة البريد الإلكتروني الوجهة.

إذا استمرت المشكلة، فقد تحتاج إلى الاتصال بمسؤول مضيف البريد الذي تحاول إرسال بريد إلكتروني إليه. دوّن الخطأ الخارجي المفصل المتوفر في رسالة الارتداد. قد لا يتمكن دعم Microsoft من المساعدة بشكل أكبر.
