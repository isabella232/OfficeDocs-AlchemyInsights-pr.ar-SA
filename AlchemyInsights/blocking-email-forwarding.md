---
title: حظر إعادة توجيه البريد الإلكتروني التلقائي الخارجي أو إلغاء حظره
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
ms.openlocfilehash: 6c4ddd53ab794ffad3179dd86a8f81785567cfe34240dff2aa0a1df11094883d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897455"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>حظر إعادة توجيه البريد الإلكتروني التلقائية أو إلغاء حظرها

لتمكين إعادة توجيه البريد الإلكتروني لعلبة بريد معينة أو تعطيلها، راجع [تكوين إعادة توجيه البريد الإلكتروني](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

يمكن للمسؤولين التحكم في إعادة توجيه خارجي المؤسسة باستخدام [سياسات البريد العشوائي الصادر.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) يمكنك إدارة سياسات البريد العشوائي الصادرة في مدخل Microsoft 365 Defender في أو باستخدام <https://security.microsoft.com/antispam> [الأمر Cmdlet Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) في Exchange Online PowerShell.

إذا تلقيت الخطأ التالي: "تم رفض **الوصول إلى 550 5.7.520،** لا تسمح مؤسستك ب إعادة توجيه خارجي"، فتأكد من تكوين النهج لتمكين الرسائل الخارجية التي تم إعادة توجيهها بشكل تلقائي.

**ملاحظة**: نوصي بالقيمة الافتراضية تلقائي **-** النظام الذي يتم التحكم فيه لإعداد قواعد إعادة توجيه تلقائية في نهج تصفية البريد العشوائي الافتراضي الصادر (يتم حظر إعادة توجيه خارجية تلقائية؛ لا تزال إعادة توجيه تلقائي داخلية تعمل).  يجب إنشاء سياسات تصفية بريد عشوائي مخصصة للبريد الصادر واستخدام القيمة **عند -** يتم تمكين إعادة توجيه فقط للمستخدمين الذين يحتاجون إلى إعادة توجيه البريد الإلكتروني التلقائي الخارجي. لمزيد من المعلومات، راجع تكوين إعادة توجيه البريد الإلكتروني [الخارجي في Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
