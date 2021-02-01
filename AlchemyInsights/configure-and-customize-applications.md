---
title: تكوين التطبيقات وتخصيصها
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063576"
---
# <a name="configure-and-customize-applications"></a>تكوين التطبيقات وتخصيصها

**تكوين التطبيقات**

1. تشغيل سريع: يمكنك تكوين خصائص تطبيق في مستأجر [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) يوضح لك كيفية تكوين بعض الخصائص لتطبيق ما.
2. للمساعدة في دمج تطبيقاتك مع Azure Active [](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) Directory، قمنا بتطوير مجموعة من البرامج التعليمية التي تساعدك على القيام بالتهيئة.
3. [تساعدك كيفية تكوين](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) تطبيق وكيل التطبيق على فهم كيفية تكوين تطبيق وكيل التطبيق ضمن Azure AD لكشف التطبيقات في الموقع على السحابة.
4. قم بتنزيل [PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)وتكوين التطبيق: اتبع الإرشادات الواردة في تكوين *PingAccess ل Azure AD* لحماية التطبيقات المنشورة باستخدام وكيل تطبيق Microsoft Azure AD على موقع Ping Identity على ويب وتنزيل الإصدار الأخير من PingAccess.

**أخطاء التطبيق التي تم تكوينها بشكل خاطئ (AADSTS650056)**

1. تأكد من أنك تقوم بالوصول إلى التطبيق من عنوان تسجيل الدخول الذي وفره مالك التطبيق. بمعنى آخر، سجل الدخول إلى التطبيق من خلال عمليتها العادية. في معظم الحالات، سيتم حل هذه المشكلة بشكل تلقائي بشكل طبيعي. إذا لم يكن كذلك، يمكن أن يساعد هذا المنشور في استكشاف الأخطاء وإصلاحها وحلها.
2. **إذا كانت مؤسستك تملك التطبيق** (مما يعني أن تسجيل التطبيق في مؤسستك):
    - على الأقل، نوصي بإذن أو تفويض من `User.Read` `openid` Microsoft **Graph.**
    - تأكد من موافقة التطبيق وجميع الأذونات الخاصة به. يمكنك التحقق من ذلك بالنظر إلى العمود **"الحالة"** الخاص بتسجيل التطبيق ضمن **"أذونات API".**
    - في بعض السيناريوهات، قد يكون التطبيق جهة خارجية ولكن قد يكون مسجلا في مؤسستك. تأكد ما إذا كان هذا التطبيق مدرجا في تسجيلات التطبيق (وليس تطبيقات المؤسسة).
    - إذا استمر رؤيه رسالة الخطأ هذه. بعد ذلك، قد تحتاج إلى إنشاء عنوان URL الموافقة الموضح في **الخطوة 4.**
3. **إذا لم تكن مؤسستك مالك التطبيق وتستخدمه كتطبيق جهة خارجية:**
    - إذا كنت المسؤول العام/الشركة، يجب أن تظهر شاشة الموافقة. تأكد من أنك قمت بالتحقق من المربع "الموافقة بالنيابة **عن مؤسستك".**
    - إذا لم تظهر شاشة الموافقة، فاحذف تطبيق Enterprise وحاول مرة أخرى.
    - إذا استمر رؤيه رسالة الخطأ هذه. بعد ذلك، قد تحتاج إلى إنشاء عنوان URL الموافقة الموضح في **الخطوة 4.**
4. إنشاء عنوان **URL** الموافقة يدويا لاستخدامه: إذا تم تصميم التطبيق للوصول إلى مورد معين، فقد لا تتمكن من استخدام أزرار الموافقة من مدخل Azure، ستحتاج إلى إنشاء URL الموافقة يدويا واستخدام هذا.
    - ستحتاج إلى الحصول على `{App-Id}` ومن `{App-Uri-Id}` مالك التطبيق. `{Tenant-Id}` سيكون معرف المستأجر الخاص بك. سيكون هذا إما `yourdomain.onmicrosoft.com` أو "هوية الدليل".
    - إذا كان التطبيق الوصول إلى نفسه للمورد، فينطبق ذلك على `{App-Id}` `{App-Uri-Id}`
5. لمزيد من المعلومات، راجع مشاكل تسجيل الدخول إلى تطبيقات تسجيل الدخول الفردية المستندة إلى [SAML التي تم تكوينها.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**تخصيص التطبيقات**

- إضافة العلامة التجارية إلى صفحة تسجيل الدخول إلى [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) الخاصة مؤسستك - استخدم شعار مؤسستك ومخططات الألوان المخصصة لتوفير شكل متناسق ومشعر لصفحات تسجيل الدخول إلى Azure Active Directory (Azure AD).
- [أضف اسم مجالك المخصص باستخدام مدخل Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) - يأتي كل مستأجر Azure AD جديد باسم مجال أولي. لا يمكنك تغيير اسم المجال الأولي أو حذفه، ولكن يمكنك إضافة أسماء مؤسستك. تساعدك إضافة أسماء مجالات مخصصة على إنشاء أسماء مستخدمين مألوفة للمستخدمين.
