---
title: 726 حظر إعادة توجيه البريد الإلكتروني
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059619"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>حظر إعادة توجيه البريد الإلكتروني أو إلغاء حظرها

لتمكين إعادة توجيه البريد الإلكتروني لعلبة بريد معينة أو تعطيلها، راجع [تكوين إعادة توجيه البريد الإلكتروني](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

على مستوى المستأجر، يتم التحكم في إعادة توجيه البريد الخارجي باستخدام نهج البريد العشوائي الصادر. يمكنك التحقق من نهج تصفية البريد العشوائي [](https://protection.office.com/antispam) الصادر من مركز الأمان والتوافق هنا أو باستخدام الأمر [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

إذا كنت تحصل على الخطأ التالي: "تم رفض **الوصول إلى 550 5.7.520،** لا تسمح مؤسستك ب إعادة توجيه خارجي"، فالرجاء التأكد من تكوين النهج لتمكين إعادة توجيه تلقائي خارجي.

**ملاحظة:** من المستحسن الاحتفاظ ب "توجيه تلقائي خارجي" معطلا على نهج تصفية البريد العشوائي الخارجي الافتراضي وتمكينه فقط للمستخدمين الذين يحتاجون إلى إعادة توجيه خارجية عن طريق إنشاء نهج مخصص لهؤلاء المستخدمين. يمكنك قراءة المزيد في تكوين إعادة توجيه البريد الإلكتروني [الخارجي في Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).