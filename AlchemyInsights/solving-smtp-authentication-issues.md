---
title: حل مشكلات مصادقة SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 814c49e8e65966a0c9f927b1f7bfb03d3dc3d637
ms.sourcegitcommit: 0e43e19448705f151846e9e9e1e0f47e12938fdf
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/15/2020
ms.locfileid: "44264303"
---
# <a name="solving-smtp-authentication-issues"></a>حل مشكلات مصادقة SMTP

إذا كنت تحصل على أخطاء 5.7.57 أو 5.7.3 عند محاولة إرسال البريد الإلكتروني SMTP والمصادقة مع عميل أو تطبيق، هناك عدد قليل من الأشياء التي يجب التحقق منها:

- قد يتم تعطيل إرسال SMTP المصادق عليه في المستأجر، أو على صندوق البريد الذي تحاول استخدامه (تحقق من كلا الإعدادين). لقراءة المزيد، راجع [تمكين أو تعطيل إرسال SMTP العميل المصادق عليه](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).

- تحقق مما إذا كانت [إعدادات أمان Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) ممكّنة للمستأجر؛ إذا تم تمكينمصادقة SMTP باستخدام المصادقة الأساسية (المعروفة أيضًا باسم Legacy؛ وهذا سيستخدم اسم المستخدم وكلمة المرور) ستفشل.
