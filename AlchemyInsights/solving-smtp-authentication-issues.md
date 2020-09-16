---
title: حل مشاكل مصادقه SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: 3eaab2c601f78e20f2ee67bc21a9598cb45a24f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737976"
---
# <a name="solving-smtp-authentication-issues"></a>حل مشاكل مصادقه SMTP

إذا كنت تتلقي أخطاء 5.7.57 أو 5.7.3 عند محاولة إرسال بريد SMTP الكتروني والمصادقة مع عميل أو تطبيق ، فهناك بعض الأمور التي يجب التحقق منها:

- قد يتم تعطيل إرسال SMTP المصادق عليه في نطاق المستاجر أو علي علبه البريد التي تحاول استخدامها (تحقق من الإعدادين). لقراءه المزيد ، راجع [تمكين إرسال SMTP للعميل المصدق أو تعطيله](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).

- تحقق مما إذا كانت [الإعدادات الافتراضية لامان Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) ممكنة للمستاجر لديك ؛ إذا كان ممكنا ، فان مصادقه SMTP باستخدام المصادقة الاساسيه (المعروفة أيضا بالقديمة ؛ سيؤدي ذلك إلى استخدام اسم المستخدم وكلمه المرور).
