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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506430"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>إصلاح مشكلات تسليم البريد الإلكتروني لرمز الخطأ 5.7.23

تحقق من سجل DNS SPF للمجال الخاص بك في مدقق سجل SPF أو DNS متوفر بشكل عام على الويب.

تحقق من أن الرسالة الصادرة لم يتم تعريفها كرسائل غير مرغوب فيها من قبل Microsoft وتم توجيهها من خلال [تجمع التسليم عالي الخطورة](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). لن تجتاز الرسائل الموجودة في تجمع التسليم عالي المخاطر شيكات SPF، وبالتالي لن يتم قبولها من قبل مؤسسة البريد الإلكتروني الوجهة.

إذا استمرت المشكلة، فقد تحتاج إلى الاتصال بمسؤول مضيف البريد الذي تحاول إرسال بريد إلكتروني إليه. دوّن الخطأ الخارجي المفصل المتوفر في رسالة الارتداد. قد لا يتمكن دعم Microsoft من المساعدة بشكل أكبر.
