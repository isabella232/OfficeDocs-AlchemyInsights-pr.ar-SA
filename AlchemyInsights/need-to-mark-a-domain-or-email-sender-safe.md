---
title: هل تحتاج إلى وضع علامة علي المجال أو مرسل البريد الكتروني بأمان ؟
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803232"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>هل تحتاج إلى وضع علامة علي المجال أو مرسل البريد الكتروني بأمان ؟

- **لا يوصي باستخدام قوائم المرسلين الموثوق** بها لأنها تفتح المؤسسة الخاصة بك بالبريد العشوائي والفيش وهجمات الانتحال.
- ومع ذلك ، إذا كان هناك متطلب شركه ، **فنوصي** باستخدام **[قواعد تدفق البريد](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** لهذا الاجراء. تضمن الإرشادات الخاصة بنا مصادقه المرسل (التحقق من ان المجال لم يتم الآن الانتحال). **ملاحظه**: لا نوصي باداره بوسيتيفيس false باستخدام قوائم المرسلين الموثوق بهم ، لأنه بإمكان الاستثناءات لتصفيه البريد العشوائي فتح مؤسستك في هجمات الأمان. إذا تلقي المستخدمون الرسائل التي تم وضع علامة عليها بشكل غير صحيح أو بريد الكتروني غير هام ، فالرجاء **[الإبلاغ عن الرسائل والملفات إلى Microsoft](https://protection.office.com/reportsubmission)**.
- **يجب تجنب** المرسلين الموثوق بهم في Outlook أو قائمه المرسلين المسموح بهم أو قائمه المجالات المسموح بها في نهج الحماية من البريد العشوائي لان المرسلين يقومون بتجاوز كل البريد العشوائي والسبووف والحماية الفيشة ومصادقه المرسل (SPF و DKIM و DMARC). يفضل استخدام هذه الطريقة للاختبار المؤقت فقط.
