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
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077638"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>تمكين مصادقة SMTP وإصلاحها

إذا كنت تريد تمكين مصادقة SMTP لعلبة بريد أو إذا كنت تحصل على رسالة الخطأ "العميل غير مصدق عليه" أو "المصادقة غير ناجحة" أو "SmtpClientAuthentication" مع الرمز 5.7.57 أو 5.7.3 أو 5.7.139 عند محاولة ترحيل البريد الإلكتروني عن طريق مصادقة جهاز أو تطبيق باستخدام Microsoft 365، يمكنك تنفيذ هذه الإجراءات الثلاثة لحل المشكلة:

1. قم [بتعطيل إعدادات أمان Azure الافتراضية](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) عن طريق تبديل **تمكين إعدادات الأمان الافتراضية** إلى **لا**.

    أ. سجل دخولك إلى مدخل Azure كمسؤول أمان أو مسؤول وصول شرطي أو مسؤول عام.<BR/>
    ب. استعرض إلى Azure Active Directory > **خصائص .**<BR/>
    ج. حدد **إدارة إعدادات الأمان الافتراضية**.<BR/>
    د. تعيين **تمكين إعدادات الأمان الافتراضية** إلى **لا**.<BR/>
    ه. حدد **حفظ**.

2. [تمكين إرسال SMTP للعميل](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) على علبة البريد المرخصة.

    أ. من مركز مسؤولي Microsoft 365، انتقل إلى **المستخدمون النشطون**، وحدد المستخدم.<BR/>
    ب. انتقل إلى علامة التبويب البريد، و ضمن **تطبيقات البريد الإلكتروني،** حدد **إدارة تطبيقات البريد الإلكتروني**.<BR/>
    د. تأكد من **أن SMTP المصادق** عليه محدد (تم تمكينه).<BR/>
    ه. حدد **حفظ التغييرات**.<BR/>

3. [قم بتعطيل المصادقة متعددة العوامل (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) على علبة البريد المرخصة.

    أ. انتقل إلى مركز مسؤولي Microsoft 365، وفي قائمة التنقل اليسرى حدد  >  **المستخدمون المستخدمون النشطون**.<BR/>
    ب. حدد **المصادقة متعددة العوامل**.<BR/>
    ج. حدد المستخدم وعطل **وثة متعددة العوامل**.<BR/>
