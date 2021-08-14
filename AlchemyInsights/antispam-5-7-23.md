---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932156"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>إصلاح مشاكل تسليم البريد الإلكتروني لرمز الخطأ 5.7.23

تحقق من سجل SPF DNS لمجالك في مدقق سجلات SPF أو DNS متوفر بشكل عام على الويب.

تحقق من أن الرسالة الصادرة لم يتم تعريفها كرسالة عشوائية من قبل Microsoft، وقد تم توجيهها عبر "تجمع التسليم [عالي المخاطر".](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) لن تجتاز الرسائل في "تجمع التسليم عالي المخاطر" عمليات التحقق من SPF، وبالتالي لن تقبلها مؤسسة البريد الإلكتروني الوجهة.

إذا استمرت المشكلة، فقد تحتاج إلى الاتصال بمسؤول مضيف البريد الذي تحاول إرسال البريد الإلكتروني إليه. دون الخطأ الخارجي المفصل المتوفر في رسالة المرتد. قد لا يتمكن دعم Microsoft من المساعدة بشكل أكبر.
