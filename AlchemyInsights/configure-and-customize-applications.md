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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044975"
---
# <a name="configure-and-customize-applications"></a>تكوين التطبيقات وتخصيصها

**تكوين التطبيقات**

1. تشغيل سريع: يوضح لك تكوين خصائص تطبيق في مستأجر [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) كيفية تكوين بعض خصائص تطبيق.
2. للمساعدة في دمج تطبيقاتك مع Azure Active [](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) Directory، قمنا بتطوير مجموعة من البرامج التعليمية التي تساعدك على عملية التكوين.
3. [تساعدك كيفية تكوين](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) تطبيق وكيل التطبيق على فهم كيفية تكوين تطبيق وكيل التطبيق ضمن Azure AD لكشف التطبيقات الموجودة على السحابة.
4. تنزيل [PingAccess وتكوين](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)التطبيق : اتبع الإرشادات الواردة في تكوين *PingAccess ل Azure AD* لحماية التطبيقات المنشورة باستخدام وكيل التطبيق Microsoft Azure AD على موقع هوية Ping على الويب وتنزيل أحدث إصدار من PingAccess.

**أخطاء التطبيق الذي تم تكوينه بشكل خاطئ (AADSTS650056)**

1. تأكد من أنك تقوم بالوصول إلى التطبيق من عنوان تسجيل الدخول الذي وفره مالك التطبيق. وبخلاف ذلك، سجل الدخول إلى التطبيق من خلال عمليتها العادية. في معظم الحالات، سيتم حل هذه المشكلة بشكل تلقائي بشكل طبيعي. إذا لم يكن كذلك، فقد يساعد هذا المنشور في استكشاف الأخطاء وإصلاحها وحلها.
2. **إذا كانت مؤسستك تملك التطبيق** (مما يعني أن تسجيل التطبيق في مؤسستك):
    - على الأقل، نوصي بالإذن أو المفوض من Microsoft Graph `User.Read` `openid` إضافة. 
    - تأكد من موافقة التطبيق وجميع الأذونات الخاصة به. يمكنك التحقق من ذلك بالنظر إلى عمود **الحالة** لتسجيل التطبيق ضمن **أذونات API**.
    - في بعض السيناريوهات، قد يكون التطبيق جهة خارجية ولكن قد يكون مسجلا في مؤسستك. تأكد من إدراج هذا التطبيق في تسجيلات التطبيق (وليس تطبيقات المؤسسة).
    - إذا استمر رؤيه رسالة الخطأ هذه. بعد ذلك، قد تحتاج إلى إنشاء عنوان URL للموافقة الموضح في **الخطوة 4**.
3. **إذا لم تكن مؤسستك مالكة التطبيق واستخدامها كتطبيق جهة خارجية:**
    - إذا كنت المسؤول العام/الشركة، يجب أن تظهر شاشة الموافقة. تأكد من أنك قمت بالتحقق من المربع "الموافقة بالنيابة **عن مؤسستك"**.
    - إذا لم تظهر شاشة الموافقة، فاحذف تطبيق Enterprise وحاول مرة أخرى.
    - إذا استمر رؤيه رسالة الخطأ هذه. بعد ذلك، قد تحتاج إلى إنشاء عنوان URL للموافقة الموضح في **الخطوة 4**.
4. إنشاء عنوان URL الموافقة يدويا لاستخدامه **:** إذا تم تصميم التطبيق للوصول إلى مورد معين، فقد لا تتمكن من استخدام أزرار الموافقة من مدخل Azure، ستحتاج إلى إنشاء عنوان URL موافقتك يدويا واستخدام هذا.
    - ستحتاج إلى الحصول على `{App-Id}` و من `{App-Uri-Id}` مالك التطبيق. `{Tenant-Id}` سيكون معرف المستأجر الخاص بك. سيكون هذا إما `yourdomain.onmicrosoft.com` أو "هوية الدليل".
    - إذا كان التطبيق في الوصول إلى نفسه للمورد، فإن `{App-Id}` و `{App-Uri-Id}` سيكونان متشابهين.
5. لمزيد من المعلومات، راجع مشاكل تسجيل الدخول إلى تطبيقات تسجيل الدخول الفردية المستندة إلى [SAML التي تم تكوينها](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**تخصيص التطبيقات**

- إضافة علامة تجارية إلى صفحة تسجيل الدخول إلى [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) في مؤسستك - استخدم شعار مؤسستك ومخططات الألوان المخصصة لتوفير شكل متناسق ومشعر لصفحات تسجيل الدخول في Azure Active Directory (Azure AD).
- [أضف اسم مجالك المخصص باستخدام مدخل Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) - يأتي اسم المجال الأولي لكل مستأجر Azure AD جديد. لا يمكنك تغيير اسم المجال الأولي أو حذفه، ولكن يمكنك إضافة أسماء مؤسستك. تساعدك إضافة أسماء مجالات مخصصة على إنشاء أسماء مستخدمين مألوفة للمستخدمين.
