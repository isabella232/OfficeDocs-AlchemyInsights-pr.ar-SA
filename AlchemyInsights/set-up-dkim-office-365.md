---
title: إعداد DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509371"
---
# <a name="setup-dkim"></a>إعداد DKIM

الإرشادات الكاملة لتكوين DKIM للمجالات المخصصة في Microsoft 365 [هنا](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. **لكل** مجال مخصص، تحتاج إلى إنشاء **سجلين** DKIM CNAME في خدمة استضافة DNS الخاصة بنطاقك (عادةً، مسجل النطاق). على سبيل المثال، تتطلب contoso.com fourthcoffee.com أربعة سجلات DKIM CNAME: اثنان contoso.com واثنين fourthcoffee.com.

   تستخدم سجلات DKIM CNAME **لكل** مجال مخصص التنسيقات التالية:

   - **اسم المضيف:**`selector1._domainkey.<CustomDomain>`

     **نقاط للعنوان أو القيمة:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **اسم المضيف:**`selector2._domainkey.<CustomDomain>`

     **نقاط للعنوان أو القيمة:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>هو النص إلى اليسار `.mail.protection.outlook.com` في سجل MX المخصص للمجال المخصص (على سبيل المثال، `contoso-com` للمجال contoso.com). \<InitialDomain\>هو المجال الذي استخدمته عند الاشتراك في Microsoft 365 (على سبيل المثال، contoso.onmicrosoft.com).

2. بعد إنشاء سجلات CNAME للمجالات المخصصة، أكمل الإرشادات التالية:

   أ. [تسجيل الدخول إلى Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) باستخدام حساب العمل أو المدرسة.

   ب. حدد رمز قاذفة التطبيق في أعلى اليسار واختر **المسؤول**.

   ج. في التنقل السفلي الأيسر، قم بتوسيع **المسؤول** واختيار **Exchange**.

   د. انتقل **Protection**إلى  >  **حماية DKIM**.

   ه. حدد المجال ثم اختر **تمكين** **رسائل التوقيع لهذا المجال مع توقيعات DKIM**. كرر هذه الخطوة لكل مجال مخصص.
