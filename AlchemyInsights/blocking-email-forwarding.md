---
title: 726 حظر أعاده توجيه البريد الكتروني
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219842"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>حظر أعاده توجيه البريد الكتروني أو إلغاء حظره

لتمكين أعاده توجيه البريد الكتروني لعلبه بريد معينه أو تعطيلها ، راجع [تكوين أعاده توجيه البريد الكتروني](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

علي مستوي المستاجر ، يتم التحكم في أعاده التوجيه الخارجي باستخدام نهج الحماية من البريد العشوائي الصادر. إذا تم تعيينه إلى إيقاف التشغيل أو التلقائي ، فقد يؤدي ذلك إلى منع أعاده توجيه البريد الكتروني باستخدام "550 5.7.520 Access التالي ، إذا تم تعيين أعاده التوجيه إلى محظور ، فهذا يعني ان الخطا سيشاهده المستخدمون.

إذا تم حظر أعاده التوجيه ، فالرجاء التاكد من تكوين النهج لتمكين الأوتوفوروارد الخارجي. يمكنك التحقق من نهج تصفيه البريد العشوائي الصادر من مركز الأمان والتوافق أو عن طريق تشغيل الأمر هوستيدوتبوندسبامفيلتيربوليسي | fl name, أوتوفورواردينجمودي. إذا كنت تريد اعداد حظر أوتوفوروارد ، سيعلمك الأمر نفسه بحاله النهج الآن.

ملاحظه: يوصي بالاحتفاظ بالأوتوفوروارد الخارجية معطلا علي نهج تصفيه البريد الكتروني الصادر الافتراضي وتمكينها فقط للمستخدمين الذين يحتاجون إلى أعاده توجيه خارجيه عن طريق إنشاء نهج مخصص لهؤلاء المستخدمين. يمكنك قراءه المزيد في [تكوين أعاده توجيه البريد الكتروني الخارجي في Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).