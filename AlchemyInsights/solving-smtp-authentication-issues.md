---
title: حل مشاكل مصادقة SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826402"
---
# <a name="solving-smtp-authentication-issues"></a>حل مشاكل مصادقة SMTP

إذا كنت تحصل على أخطاء 5.7.57 أو 5.7.3 عند محاولة إرسال بريد SMTP الإلكتروني والمصادقة مع عميل أو تطبيق، فهناك بعض الأمور التي يجب التحقق من صحتها:

- قد يتم تعطيل إرسال SMTP المصادق عليه في المستأجر أو في علبة البريد التي تحاول استخدامها (تحقق من الإعدادين). لقراءة المزيد، راجع [تمكين إرسال SMTP](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)للعميل المصادق عليه أو تعطيله .

- تحقق مما إذا [كانت إعدادات أمان Azure الافتراضية](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) تم تمكينها للمستأجر الخاص بك؛ إذا تم تمكينها، ستفشل مصادقة SMTP باستخدام المصادقة الأساسية (المعروفة أيضا باسم القديمة؛ حيث سيستخدم هذا اسم المستخدم وكلمة المرور).
