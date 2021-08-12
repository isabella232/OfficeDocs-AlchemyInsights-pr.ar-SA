---
title: تمكين مصادقة SMTP وإصلاحها
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
ms.openlocfilehash: f6f0228f6cdf7e07c9f439c54a7a2bd5364381c0e47dc80117bd964c5eafea61
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957195"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>تمكين مصادقة SMTP وإصلاحها

إذا كنت تريد تمكين مصادقة SMTP لعلبة بريد أو إذا كنت تحصل على رسالة الخطأ "العميل غير مصدق عليه" أو "المصادقة غير ناجحة" أو "SmtpClientAuthentication" مع الرمز 5.7.57 أو 5.7.3 أو 5.7.139 عند محاولة ترحيل البريد الإلكتروني عن طريق مصادقة جهاز أو تطبيق باستخدام Microsoft 365، يمكنك تنفيذ هذه الإجراءات الثلاثة لحل المشكلة:

1. قم [بتعطيل إعدادات أمان Azure الافتراضية](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) عن طريق تبديل **تمكين إعدادات الأمان الافتراضية** إلى **لا**.

    a. سجل دخولك إلى مدخل Azure كمسؤول أمان أو مسؤول وصول شرطي أو مسؤول عام.<BR/>
    b. استعرض إلى Azure Active Directory > **خصائص .**<BR/>
    c. حدد **إدارة إعدادات الأمان الافتراضية**.<BR/>
    d. تعيين **تمكين إعدادات الأمان الافتراضية** إلى **لا**.<BR/>
    e. حدد **حفظ**.

2. [تمكين إرسال SMTP للعميل](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) على علبة البريد المرخصة.

    a. من مركز مسؤولي Microsoft 365، انتقل إلى **المستخدمون النشطون**، وحدد المستخدم.<BR/>
    b. انتقل إلى علامة التبويب البريد، و ضمن **تطبيقات البريد الإلكتروني،** حدد **إدارة تطبيقات البريد الإلكتروني**.<BR/>
    d. تأكد من **أن SMTP المصادق** عليه محدد (تم تمكينه).<BR/>
    e. حدد **حفظ التغييرات**.<BR/>

3. [قم بتعطيل المصادقة متعددة العوامل (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) على علبة البريد المرخصة.

    a. انتقل إلى مركز مسؤولي Microsoft 365، وفي قائمة التنقل اليسرى حدد  >  **المستخدمون المستخدمون النشطون**.<BR/>
    b. حدد **المصادقة متعددة العوامل**.<BR/>
    c. حدد المستخدم وعطل **وثة متعددة العوامل**.<BR/>
