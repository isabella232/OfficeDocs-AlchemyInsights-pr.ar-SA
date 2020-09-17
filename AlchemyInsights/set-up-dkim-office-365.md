---
title: اعداد DKIM
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
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808694"
---
# <a name="setup-dkim"></a>اعداد DKIM

تتوفر الإرشادات الكاملة لتكوين العلامات الخاصة ب DKIM خاصه بالمجالات المخصصة في Microsoft 365 [هنا](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. بالنسبة إلى **كل** مجال مخصص ، تحتاج إلى إنشاء **سجلي CNAME لوحدتي** الأشرف في خدمه استضافه DNS الخاصة بمجالك (عاده ما يكون مسجل المجال). علي سبيل المثال ، يتطلب contoso.com و fourthcoffee.com أربعه سجلات CNAME للحصول علي اليم: اثنين لcontoso.com واثنين لfourthcoffee.com.

   تستخدم سجلات "العلامات الأشرف" ل **dkim كل** مجال مخصص التنسيقات التالية:

   - **اسم المضيف**: `selector1._domainkey.<CustomDomain>`

     **يشير إلى العنوان أو القيمة**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **اسم المضيف**: `selector2._domainkey.<CustomDomain>`

     **يشير إلى العنوان أو القيمة**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> النص إلى اليمين `.mail.protection.outlook.com` في سجل MX المخصص للمجال المخصص (علي سبيل `contoso-com` المثال ، لمجال contoso.com). \<InitialDomain\> هو المجال الذي استخدمته عند التسجيل في Microsoft 365 (علي سبيل المثال ، contoso.onmicrosoft.com).

2. بعد إنشاء سجلات CNAME للمجالات المخصصة ، أكمل الإرشادات التالية:

   علي. [سجل دخولك إلى Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) باستخدام حساب العمل أو المؤسسة التعليمية.

   ب. حدد أيقونه مشغل التطبيق في الزاوية العلوية اليمني واختر **المسؤول**.

   ن. في جزء التنقل السفلي الأيمن ، قم بتوسيع **المسؤول** واختر **Exchange**.

   ثلاثي. انتقل إلى **حماية**  >  **dkim**.

   ه. حدد المجال ، ثم اختر **تمكين** **التوقيع علي الرسائل لهذا المجال بواسطة التواقيع التي تضم اليم إلى dkim** كرر هذه الخطوة لكل مجال مخصص.
