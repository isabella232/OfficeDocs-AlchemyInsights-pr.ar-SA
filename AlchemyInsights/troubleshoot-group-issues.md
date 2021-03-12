---
title: استكشاف مشاكل المجموعة وإصلاحها
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "50713275"
---
# <a name="troubleshoot-group-issues"></a>استكشاف مشاكل المجموعة وإصلاحها

**أحتاج إلى تعيين مجموعة إلى دور Azure AD**

لتعيين مجموعة Azure Active Directory (AD) إلى دور Azure AD، قم بتنفيذ الخطوات التالية:

1. إنشاء مجموعة جديدة - لإنشاء مجموعة جديدة:

    أ. سجل الدخول إلى مركز إدارة Azure AD باستخدام أذونات مسؤول الدور المميز أو المسؤول العام. 
    ب. حدد Azure Active Directory > مجموعات > كل المجموعات > جديدة. 
    ج. إنشاء المجموعة.

2. قم بتعيين الدور إلى المجموعة إما أثناء إنشاء المجموعة أو بعد إنشائها.

    أ. لتعيين دور إلى المجموعة في وقت إنشاء المجموعة، يمكنك تبديل أدوار Azure AD إلى المجموعة وإنشاء المجموعة.
    ب. لتعيين دور إلى المجموعة بعد إنشائها، انتقل إلى علامة التبويب "الأدوار المعينة" للمجموعة التي تم إنشاؤها حديثا، ثم قم بتعيين الدور إلى المجموعة.

**أحتاج إلى إدارة عضوية مجموعة تم تعيينها إلى دور Azure AD**

1. لمنع رفع الامتيازات، بشكل افتراضي، يمكن لمسؤول الدور المميز والمسؤول العام فقط تعديل عضوية مجموعة معينة إلى دور. ومع ذلك، يمكنهم اختيار تعيين مالك لهذه المجموعة وتفويض هذه المهمة. لمزيد من المعلومات، راجع استخدام [مجموعات السحابة لإدارة تعيينات الدور في Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)
2. للأسئلة الشائعة وتلميحات استكشاف الأخطاء وإصلاحها لتعيين أدوار إلى مجموعات في Azure AD، راجع استكشاف الأخطاء وإصلاحها الأدوار المعينة إلى [مجموعات السحابة.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)

**المجموعات الديناميكية**

1. إذا لم تتمكن من العثور على سمات المستخدم المضمنة، فتأكد من وجود السمة في قائمة الخصائص المعتمدة.
2. إذا كنت تبحث عن سمات الجهاز المضمنة، فتأكد من أن السمة في قائمة سمات الجهاز 
3. بالإضافة إلى سمات المستخدم والجهاز المضمنة، يمكنك أيضا استخدام ["سمات](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties)الملحق". بعد مزامنة سمات الملحقات من Windows Server AD أو من تطبيق SaaS متصل، يجب أن تكون السمات مرئية في القائمة المنسدل منشئ القواعد. يمكن العثور على اسم السمة المخصصة في الدليل عن طريق الاستعلام عن سمة المستخدم باستخدام PowerShell والبحث عن اسم السمة. يمكن استخدام هذه أيضا عند إنشاء قواعد في بناء جملة القاعدة.
4. تأكد من أن المستأجر الخاص بك لديه الترخيص المناسب. تتطلب المجموعات الديناميكية من المستأجر الحصول على ترخيص Azure AD P1 Premium. يمكن الوصول إلى قائمة خطط ترخيص Azure AD [هنا.](https://azure.microsoft.com/pricing/details/active-directory/) يمكن الوصول إلى خطط ترخيص Enterprise Mobility + Security [هنا.](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)
5. تأكد من أن دور المستخدم الذي يقوم بإنشاء المجموعة الديناميكية هو مسؤول عام أو مسؤول intune أو مسؤول مجموعة أو مسؤول مستخدم.
6. يرجى السماح للوقت الذي يجب أن ت نشره فيه المجموعة. قد تستغرق المجموعة ما يصل إلى 24 ساعة لملء المستأجر للمرة الأولى أو بعد تغيير القاعدة، وهذا يتوقف على حجم المستأجر.
7. لمزيد من المعلومات، راجع إنشاء قواعد [تستند إلى السمات لعضوية المجموعة الديناميكية.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)

**أحتاج إلى حذف مجموعة**

1. يمكن حذف المجموعات من الدليل باستخدام الأمر Remove-AzureADGroup cmdlet في وحدة Azure AD Powershell النمطية.
2. قبل محاولة حذف مجموعة متزامنة في Azure AD، تأكد من حذف جميع التراخيص المعينة لتجنب الأخطاء.
3. لمزيد من المعلومات حول حذف المجموعات، راجع [حذف مجموعة ذات ترخيص تم تعيينه.](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)

**أحتاج إلى استعادة مجموعة محذوفة**

1. إذا تم حذف مجموعة Office 365، لا يمكن استعادتها إلا قبل 30 يوما من حدوث الحذف الدائم. بعد الحذف الدائم، لن يعود من الممكن استعادة المجموعة. تعرف على المزيد حول استعادة المجموعات [هنا.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)
2. هذه الوظيفة غير معتمدة لمجموعات الأمان ومجموعات التوزيع.
3. تأكد من أنك مفوض لاستعادة مجموعة Office 365. يمكن للمسؤولين العامين، مسؤولي المجموعات، مسؤولي حسابات المستخدمين، مسؤولي خدمة intune، دعم المستوى 1 أو الطبقة 2، ومالك المجموعة استعادة مجموعة.
4. عند حذف مجموعة ديناميكية واستعادتها، يتم النظر إليها كمجموعة جديدة وإعادة ملؤها وفقا للقاعدة. قد تستغرق هذه العملية ما يصل إلى 24 ساعة.
5. لمزيد من المعلومات حول استعادة مجموعة محذوفة، راجع استعادة مجموعة Office 365 محذوفة [في Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**تكوين نهج انتهاء صلاحية المجموعة**

1. هذه الوظيفة معتمدة لمجموعات Office 365 فقط، وليس لمجموعات الأمان ومجموعات التوزيع غير معتمدة.
2. يتطلب تكوين نهج انتهاء الصلاحية لمجموعات Office 365 واستخدامه ترخيص Azure AD Premium.
3. يمكن حاليا تكوين نهج انتهاء صلاحية واحد فقط لمجموعات Office 365 على مستأجر.
4. يمكن فقط للمسؤولين العامين، مسؤولي المجموعة، مسؤولي المستخدمين ومالك المجموعة تجديد المجموعة.
5. إذا انتهت صلاحية مجموعة Office 365، يتم حذفها ولا يمكن استعادتها إلا قبل 30 يوما من حدوث الحذف الدائم. بعد الحذف الدائم، لن يعود من الممكن استعادة المجموعة. تعرف على المزيد حول استعادة المجموعات [هنا.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**التجديد التلقائي المستند إلى النشاط**

يمكن لأنشطة المستخدم من SharePoint و Outlook و Teams تشغيل التجديد التلقائي للمجموعة. يتم التحقق من الأنشطة قبل 35 يوما من انتهاء صلاحية المجموعة. إذا كان هناك نشاط خلال دورة حياة المجموعة الحالية، سيتم تجديد المجموعة تلقائيا ولن يتم إرسال إعلام البريد الإلكتروني إلى مالكي المجموعة.

**توقيت الإعلامات للمجموعات منتهية الصلاحية**

1. يتم إرسال إعلامات البريد الإلكتروني إلى مالكي مجموعة Office 365 قبل انتهاء صلاحية المجموعة ب 30 يوما و15 يوما ويوم واحد.
2. عند إعداد انتهاء الصلاحية للمرة الأولى، يتم تعيين أي مجموعات أقدم من فاصل انتهاء الصلاحية إلى 35 يوما حتى انتهاء الصلاحية.
3. يتم حساب تاريخ انتهاء صلاحية المجموعة استنادا إلى تاريخ تجديد المجموعة، ولا يستند إلى تاريخ تحديث النهج. إذا تم تحديث نهج انتهاء الصلاحية، لن يتغير تاريخ انتهاء الصلاحية.
4. لمزيد من المعلومات، راجع نهج انتهاء صلاحية المجموعة ورسائل البريد الإلكتروني للتجديد واستعادة مجموعة Office 365 محذوفة [في Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted) [](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle)

**الإذن لإنشاء مجموعة**

تأكد من أنك مفوض لإنشاء مجموعة جديدة. يمكن للمسؤولين العامين تعطيل إنشاء المجموعة في مدخل Azure أو لوحة Access. قد تحتاج إلى مسؤول لإنشاء المجموعة الجديدة لك، أو من أجل من يعطيك الأذونات المناسبة.

1. [إنشاء مجموعة جديدة وإضافة أعضاء في مدخل Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [إنشاء مجموعات في Powershell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [تعطيل إنشاء المجموعات في Powershell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [إدارة الأشخاص الذين يمكنهم إنشاء مجموعات في Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [تعطيل إعلام الترحيب في Office 365 عبر Powershell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [أدوار Azure AD الإدارية](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**إدارة أذونات إنشاء المجموعة**

1. يمكن للمسؤولين العامين إدارة أذونات إنشاء مجموعة الأمان أو مجموعات Office 365 التي تم إنشاؤها في مدخل Azure أو لوحة الوصول، عن طريق تعيين المستخدمين الذين يمكنهم إنشاء مجموعات أمان في مداخل **Azure** أو يمكن للمستخدمين إنشاء مجموعات **Office 365** في إعدادات مداخل Azure في كل المجموعات **> العامة (الإعدادات).**
2. يمكنك أيضا تقييد إنشاء المجموعة لتحديد مجموعة من المستخدمين إذا كان لديك ترخيص Azure AD P1 Premium.

**تعطيل إعلام الترحيب للأعضاء الجدد في مجموعة Office 365**

يمكن تعطيل إعلام الترحيب المرسل إلى المستخدمين الذين تم إضافتهم إلى مجموعات Office 365 عن طريق تعيينه إلى `UnifiedGroupWelcomeMessageEnabled` **"خطأ"** في Powershell. تعرف على هذا الإعداد [هنا.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)













