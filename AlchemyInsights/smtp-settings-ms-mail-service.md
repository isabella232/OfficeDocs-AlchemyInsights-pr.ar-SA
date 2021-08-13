---
title: إعدادات SMTP لخدمة Microsoft 365 البريد الإلكتروني
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: 373042e9593faf4eaa486313763beb8e8f48b6e9ea159d1cfb37b9df826384f4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813964"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>إعدادات SMTP لخدمة Microsoft 365 البريد الإلكتروني

هذه هي إعدادات SMTP لخدمات Microsoft 365 البريد:

**الخادم**: smtp.office365.com </br>
**المنفذ**: 587 </br>
**التشفير**: STARTTLS (يتم دعم إصدار TLS 1.2 فقط الآن. يرجى التأكد من أن التطبيق أو الجهاز يدعم TLS 1.2) </br>
**اسم** المستخدم : عنوان Office 365 الخاص بك (على سبيل المثال، example@yourdomain.com) </br>
**كلمة** المرور : كلمة Office 365 المرور </br>
**المصادقة**: مطلوب </br>
**حدود الإرسال**: 10000 رسالة بريد إلكتروني في اليوم </br>

للحصول على إعدادات POP و IMAP، راجع [إعدادات POP و IMAP و SMTP](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353).
 
للتعرف على خيارات ترحيل البريد الإلكتروني باستخدام Microsoft 365 والخطوات، راجع كيفية إعداد جهاز أو تطبيق متعدد الوظائف لإرسال البريد الإلكتروني باستخدام Microsoft 365 [أو Office 365](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).