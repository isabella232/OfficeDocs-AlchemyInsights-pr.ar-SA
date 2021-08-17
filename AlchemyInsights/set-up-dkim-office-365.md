---
title: إعداد DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108543"
---
# <a name="setup-dkim"></a>إعداد DKIM

الإرشادات الكاملة لتكوين DKIM للمجالات المخصصة في Microsoft 365 [هنا](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. لكل **مجال** مخصص، تحتاج إلى إنشاء سجلي **DKIM** CNAME في خدمة استضافة DNS لمجالك (عادة ما تكون جهة تسجيل المجالات). على سبيل المثال contoso.com يتطلب fourthcoffee.com DKIM CNAME أربعة سجلات: سجلان contoso.com واثنان fourthcoffee.com.

   تستخدم سجلات DKIM CNAME **لكل** مجال مخصص التنسيقات التالية:

   - **اسم المضيف**: `selector1._domainkey.<CustomDomain>`

     **يشير إلى العنوان أو القيمة**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **اسم المضيف**: `selector2._domainkey.<CustomDomain>`

     **يشير إلى العنوان أو القيمة**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> هو النص إلى يسار في سجل MX المخصص للمجال المخصص (على سبيل المثال، `.mail.protection.outlook.com` `contoso-com` للمجال contoso.com). \<InitialDomain\>هو المجال الذي استخدمته عند تسجيل Microsoft 365 (على سبيل المثال، contoso.onmicrosoft.com).

2. بعد إنشاء سجلات CNAME للمجالات المخصصة، أكمل الإرشادات التالية:

   a. [سجل الدخول Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) باستخدام حساب العمل أو المدرسة.

   b. حدد أيقونة شريط التطبيقات في الزاوية العلوية اليمنى واختر **المسؤول**.

   c. في التنقل السفلي الأيسر، قم بتوسيع **المسؤول** **واختر** Exchange .

   d. انتقل إلى **Protection**  >  **DKIM**.

   e. حدد المجال ثم اختر **تمكين** **لتوقيع رسائل لهذا المجال باستخدام تواقيع DKIM**. كرر هذه الخطوة لكل مجال مخصص.
