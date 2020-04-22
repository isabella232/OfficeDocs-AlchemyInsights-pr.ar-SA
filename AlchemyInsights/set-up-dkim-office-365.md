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
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645659"
---
# <a name="setup-dkim"></a>إعداد DKIM

الإرشادات الكاملة لتكوين DKIM للمجالات المخصصة في Microsoft 365 [هنا](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. **لكل** مجال مخصص، تحتاج إلى إنشاء **سجلين** DKIM CNAME في خدمة استضافة DNS الخاصة بنطاقك (عادةً، مسجل النطاق). على سبيل المثال، تتطلب contoso.com fourthcoffee.com أربعة سجلات DKIM CNAME: اثنان contoso.com واثنين fourthcoffee.com.

   تستخدم سجلات DKIM CNAME **لكل** مجال مخصص التنسيقات التالية:

   - **اسم المضيف:**`selector1._domainkey.<CustomDomain>`

     **نقاط للعنوان أو القيمة:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **اسم المضيف:**`selector2._domainkey.<CustomDomain>`

     **نقاط للعنوان أو القيمة:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> هو النص إلى `.mail.protection.outlook.com` اليسار في سجل MX المخصص للمجال المخصص `contoso-com` (على سبيل المثال، للمجال contoso.com). \<Domain\> هو المجال الذي استخدمته عند الاشتراك في Microsoft 365 (على سبيل المثال، contoso.onmicrosoft.com).

2. بعد إنشاء سجلات CNAME للمجالات المخصصة، أكمل الإرشادات التالية:

   أ. [تسجيل الدخول إلى Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) باستخدام حساب العمل أو المدرسة.

   ب. حدد رمز قاذفة التطبيق في أعلى اليسار واختر **المسؤول**.

   ج. في التنقل السفلي الأيسر، قم بتوسيع **المسؤول** واختيار **Exchange**.

   د. انتقل إلى **حماية** > **DKIM**.

   ه. حدد المجال ثم اختر **تمكين** **رسائل التوقيع لهذا المجال مع توقيعات DKIM**. كرر هذه الخطوة لكل مجال مخصص.
