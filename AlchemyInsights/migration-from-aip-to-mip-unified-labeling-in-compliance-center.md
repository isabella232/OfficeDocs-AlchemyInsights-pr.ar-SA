---
title: الترحيل من AIP إلى ميب/التسمية الموحدة في مركز التوافق
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674313"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>الترحيل من AIP إلى ميب/التسمية الموحدة في مركز التوافق

للترحيل من AIPات IP إلى التسمية الموحدة في مركز الأمان والتوافق ، قم بما يلي:

**تنشيط الحماية من مدخل Azure**

1. إذا لم تكن قد فعلت ذلك بعد ، فافتح نافذه مستعرض جديده وقم [بتسجيل الدخول إلى مدخل Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). انتقل إلى ريش **حماية البيانات في Azure** . علي سبيل المثال ، في قائمه الموزع ، انقر فوق **كافة الخدمات** وأبدا بكتابه **المعلومات** في المربع عامل التصفية. حدد **حماية البيانات في Azure**. إذا لم تكن قد قمت بالوصول إلى ريش حماية البيانات في Azure قبل ذلك ، فراجع [الخطوات الاضافيه لمره واحده](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) لأضافه هذا الريش إلى المدخل. لفتح ريش حماية البيانات في Azure ، يجب ان يتوفر لديك [خطه Premium لحماية البيانات في azure](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) أو خطه Office 365 التي تتضمن أداره الحقوق. إذا كان لديك أحد هذه الاشتراكات ولكنك تري رسالة تفيد بتعذر العثور علي اشتراك صحيح ، [فاتصل بدعم Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) أو استخدم قنوات الدعم القياسية الخاصة بك.

2. حدد موقع خيارات القائمة **أداره** ، وحدد **تنشيط الحماية**. انقر فوق **تنشيط**، ثم قم بتاكيد الاجراء. عند اكتمال عمليه التنشيط ، يعرض شريط المعلومات **انتهاء التنشيط بنجاح**.

**ترحيل تسميات حماية البيانات في Azure إلى مركز توافق & أمان Office 365**

1. تاكد من انك قمت بتسجيل الدخول كمستخدم لديه اذن المسؤول العام.

2. انتقل إلى ريش **حماية البيانات في Azure** .

3. من خيار القائمة **أداره** ، حدد **التسمية الموحدة**.

4. في **حماية البيانات في Azure-النصليه التسمية الموحدة** ، انقر فوق **تنشيط** واتبع الإرشادات الموجودة علي الإنترنت.

**ملاحظه**: تحقق من ان لديك الأذونات المناسبة قبل تنشيط ترحيل مركز توافق & الأمان. راجع هذه المقالات للحصول علي مزيد من المعلومات:

1. [هل تحتاج إلى ان تكون مسؤولا عاما لتكوين حماية البيانات في Azure ، ام يمكنني التفويض بالمسؤولين الآخرين ؟](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [معلومات مهمة حول الأدوار الاداريه بعد الترحيل إلى مركز توافق & الأمان.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

للحصول علي مزيد من المعلومات حول ترحيل التسمية الموحدة إلى مركز الأمان والتوافق ، راجع [ترحيل التسميات](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
