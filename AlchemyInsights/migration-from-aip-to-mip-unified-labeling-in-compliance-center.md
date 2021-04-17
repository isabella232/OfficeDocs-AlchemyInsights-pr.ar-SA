---
title: الترحيل من AIP إلى تسمية MIP/الموحدة في مركز التوافق
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
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825358"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>الترحيل من AIP إلى تسمية MIP/الموحدة في مركز التوافق

للترحيل من تسميات AIP إلى التسمية الموحدة في مركز الأمان والتوافق، يمكنك القيام بما يلي:

**تنشيط الحماية من مدخل Azure**

1. إذا لم تكن قد فعلت ذلك بعد، فافتح نافذة مستعرض جديدة ثم [سجل الدخول إلى مدخل Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). انتقل إلى **شفرة Azure Information Protection.** على سبيل المثال، في قائمة الموزع، انقر فوق **كافة الخدمات** وابدأ بكتابة **المعلومات** في المربع عامل التصفية. حدد **Azure Information Protection**. إذا لم تكن قد قمت بالوصول إلى شفرة Azure Information [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) Protection من قبل، فشاهد الخطوات الإضافية مرة واحدة لإضافة هذا النصل إلى المدخل. لفتح شفرة Azure Information Protection، يجب أن يكون لديك خطة [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) أو خطة Office 365 التي تتضمن إدارة الحقوق. إذا كان لديك أحد هذه الاشتراكات ولكنك رأيت رسالة بأنه يتعذر العثور على اشتراك صالح، فاتصل ب [دعم Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) أو استخدم قنوات الدعم القياسية.

2. حدد خيارات **القائمة إدارة،** وحدد **تنشيط الحماية**. انقر **فوق** تنشيط ، ثم قم بتأكيد الإجراء. عند اكتمال التنشيط، يعرض شريط المعلومات انتهاء **التنشيط بنجاح**.

**ترحيل تسميات Azure Information Protection إلى مركز & أمان Office 365**

1. تأكد من تسجيل دخولك كمستخدم بإذن المسؤول العام.

2. انتقل إلى **شفرة Azure Information Protection.**

3. من خيار **القائمة إدارة،** حدد **تسمية موحدة**.

4. على **شفرة حماية معلومات Azure - تسمية** موحدة، انقر فوق **تنشيط** واتبع الإرشادات عبر الإنترنت.

**ملاحظة:** تحقق من أن لديك الأذونات المناسبة قبل تنشيط & مركز التوافق. لمزيد من المعلومات، راجع هذه المقالات:

1. [هل تحتاج إلى أن تكون مسؤولا عاما لتكوين Azure Information Protection، أو هل يمكنني التفويض إلى مسؤولي آخرين؟](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [معلومات مهمة حول الأدوار الإدارية بعد عملية إعادة & مركز التوافق.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

لمزيد من المعلومات حول ترحيل AIP إلى التسميات الموحدة إلى مركز الأمان والتوافق، راجع [ترحيل التسميات](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
