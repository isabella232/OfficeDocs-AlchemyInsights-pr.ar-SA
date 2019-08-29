---
title: إعداد DKIM في Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666251"
---
# <a name="setup-dkim-in-office-365"></a>إعداد DKIM في Office 365

إرشادات كاملة حول تكوين DKIM للمجالات المخصصة في Office 365 [هنا](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. **كل** مجال مخصص، تحتاج إلى إنشاء **جهازي** سجلات DKIM CNAME على المجال DNS خدمة استضافة (عادة، المسجل المجال). على سبيل المثال، تتطلب contoso.com و fourthcoffee.com أربعة سجلات DKIM CNAME: اثنان ل contoso.com واثنان من fourthcoffee.com.

   استخدام سجلات DKIM CNAME **كل** مجال مخصص التنسيقات التالية:

   - **اسم المضيف**:`selector1._domainkey.<CustomDomain>`

     **يشير إلى عنوان أو القيمة**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **اسم المضيف**:`selector2._domainkey.<CustomDomain>`

     **يشير إلى عنوان أو القيمة**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> النص إلى اليسار `.mail.protection.outlook.com` في السجل MX المخصصة للمجال المخصص (على سبيل المثال، `contoso-com` ل contoso.com المجال). \<إينيتيالدومين\> هي المجال الذي تستخدمه عند اشتراكك في Office 365 (على سبيل المثال، contoso.onmicrosoft.com).

2. بعد أن قمت بإنشاء سجلات CNAME للمجالات المخصصة الخاصة بك، أكمل الإرشادات التالية:

   أ. [تسجيل الدخول إلى Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) باستخدام حسابك العمل أو المدرسة.

   (ب). حدد رمز التطبيق المشغل في الزاوية العليا اليسرى واختر **المسؤول**.

   (ج). في شريط التنقل الأيسر السفلي، قم بتوسيع **الإدارة** واختر **تبادل**.

   (د). انتقل إلى **حماية** > **DKIM**.

   (ه). حدد المجال، ثم اختر **تمكين** **توقيع الرسائل لهذا المجال بتوقيعات DKIM**. كرر هذه الخطوة لكل مجال مخصص.
