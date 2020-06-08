---
title: الترحيل من AIP إلى MIP /وضع العلامات الموحدة في مركز الامتثال
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7ce9c387fc94f59674a922c5fe071fc0fb030344
ms.sourcegitcommit: e6d73d240669342fde9d4d25b0ee2838b7e43965
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/14/2020
ms.locfileid: "44236294"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>الترحيل من AIP إلى MIP /وضع العلامات الموحدة في مركز الامتثال

للترحيل من تسميات AIP إلى وضع العلامات الموحدة في مركز الأمان والامتثال، قم بما يلي:

**تفعيل الحماية من بوابة Azure**

1. إذا لم تكن قد فعلت ذلك بالفعل، افتح نافذة متصفح جديدة [وسجّل الدخول إلى بوابة Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). انتقل إلى شفرة **حماية المعلومات Azure.** على سبيل المثال، في قائمة لوحة الوصل، انقر فوق **كافة الخدمات** وابدأ في كتابة **المعلومات** في مربع عامل التصفية. حدد **حماية معلومات Azure**. إذا لم تكن قد قمت بالوصول إلى شفرة حماية المعلومات Azure من قبل، فراجع [الخطوات الإضافية](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) لمرة واحدة لإضافة هذا النصل إلى المدخل. لفتح شفرة حماية المعلومات Azure، يجب أن يكون لديك [إما خطة Azure لحماية المعلومات أو](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) خطة Office 365 التي تتضمن إدارة الحقوق. إذا كان لديك أحد هذه الاشتراكات ولكن راجع رسالة تفيد بأنه لا يمكن العثور على اشتراك صالح، [فاتصل بدعم Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) أو استخدم قنوات الدعم القياسية.

2. تحديد موقع خيارات القائمة **إدارة،** وحدد **تنشيط الحماية**. انقر فوق **تنشيط**، ثم تأكيد الإجراء الخاص بك. عند اكتمال التنشيط، يعرض شريط المعلومات **التنشيط الذي تم الانتهاء منه بنجاح**.

**ترحيل تسميات حماية معلومات Azure إلى مركز التوافق & الأمان في Office 365**

1. تأكد من تسجيل الدخول كمستخدم بإذن المسؤول العمومي.

2. انتقل إلى شفرة **حماية المعلومات Azure.**

3. من خيار **إدارة** القائمة، حدد **وضع العلامات الموحدة**.

4. على حماية المعلومات Azure - شفرة **وضع العلامات الموحدة،** انقر فوق **تنشيط** واتبع الإرشادات عبر الإنترنت.

**ملاحظة:** تحقق من أن لديك الأذونات المناسبة قبل تنشيط ترحيل مركز التوافق & الأمان. راجع هذه المقالات لمزيد من المعلومات:

1. [هل تحتاج إلى أن تكون مسؤولًا عالميًا لتكوين حماية معلومات Azure، أم يمكنني التفويض إلى مسؤولين آخرين؟](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [معلومات هامة حول الأدوار الإدارية بعد الترحيل إلى مركز التوافق & الأمان.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

لمزيد من المعلومات حول ترحيل AIP إلى وضع العلامات الموحدة إلى مركز الأمان والامتثال، راجع [ترحيل التسميات](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
