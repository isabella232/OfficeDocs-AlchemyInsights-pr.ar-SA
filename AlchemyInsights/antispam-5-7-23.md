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
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821398"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>إصلاح مشاكل تسليم البريد الإلكتروني لرمز الخطأ 5.7.23

تحقق من سجل SPF DNS لمجالك في مدقق سجلات SPF أو DNS متوفر بشكل عام على الويب.

تحقق من أن الرسالة الصادرة لم يتم تعريفها كرسالة عشوائية من قبل Microsoft، وقد تم توجيهها عبر "تجمع التسليم [عالي المخاطر".](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) لن تجتاز الرسائل في "تجمع التسليم عالي المخاطر" عمليات التحقق من SPF، وبالتالي لن تقبلها مؤسسة البريد الإلكتروني الوجهة.

إذا استمرت المشكلة، فقد تحتاج إلى الاتصال بمسؤول مضيف البريد الذي تحاول إرسال البريد الإلكتروني إليه. دون الخطأ الخارجي المفصل المتوفر في رسالة المرتد. قد لا يتمكن دعم Microsoft من المساعدة بشكل أكبر.
