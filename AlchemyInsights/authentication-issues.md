---
title: مشكلات المصادقة
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976836"
---
# <a name="authentication-issues"></a>مشكلات المصادقة

**هل تبحث عن معلومات حول رموز خطأ AADSTS التي تم إرجاعها من خدمة رمز أمان Azure Active Directory (Azure AD) (STS)؟** راجع [مصادقة Azure AD ورموز خطأ التخويل](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) للعثور على أوصاف أخطاء AADSTS والإصلاحات وبعض الحلول البديلة المقترحة.

يمكن أن تكون أخطاء التخويل نتيجة للعديد من المشكلات المختلفة، والتي ينتج عن معظمها خطأ 401 أو 403. على سبيل المثال، يمكن أن تؤدي المشكلات التالية إلى حدوث أخطاء في التخويل:

- [تدفقات الحصول على الرمز المميز للوصول](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) غير صحيحة 
- [نطاقات الأذونات](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) تم تكوينها بشكل غير صحيح 
- عدم [الموافقة](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

لحل أخطاء التخويل الشائعة، جرّب الخطوات الموضحة أدناه والتي تتطابق بشكل وثيق مع الخطأ الذي تتلقاه. قد يتم تطبيق أكثر من خطوة لحل الخطأ الذي تتلقاه.

**401 خطأ غير مخوّل: هل رمزك المميز صالح؟**

تأكد من أن تطبيقك يقدم رمز وصول صالحًا إلى Microsoft Graph كجزء من الطلب. غالبًا ما يعني هذا الخطأ أن رمز الوصول قد يكون مفقودًا في رأس صفحة طلب مصادقة HTTP أو أن الرمز المميز غير صالح أو انتهت صلاحيته. نوصي بشدة باستخدام مكتبة مصادقة Microsoft (MSAL) للحصول على رمز الوصول. بالإضافة إلى ذلك، قد يحدث هذا الخطأ إذا حاولت استخدام رمز وصول مخوّل ممنوح لحساب Microsoft الشخصي للوصول إلى API التي تدعم فقط حسابات العمل، أو المدرسة (حسابات المؤسسة).

**403 خطأ ممنوع: هل اخترت المجموعة المناسبة من الأذونات؟**

تأكد من أنك طلبت المجموعة المناسبة من الأذونات بناءً على وحدات API لـ Microsoft Graph التي تستدعيها تطبيقاتك. يتم توفير الأذونات الموصى بها الأقل امتيازًا في جميع موضوعات أسلوب مرجع API لـ Microsoft Graph. بالإضافة إلى ذلك، يجب أن يتم منح تلك الأذونات للتطبيق من قبل مستخدم أو مسؤول. يحدث منح الأذونات عادةً من خلال صفحة الموافقة، أو استخدام شفرة تسجيل تطبيق مدخل Azure. من شفرة **الإعدادات** للتطبيق، انقر فوق **الأذونات المطلوبة**، ثم انقر فوق **منح الأذونات**. لمزيد من المعلومات، اطلع على:

- [أذونات Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [فهم أذونات Azure AD والموافقة عليها](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**الخطأ 403 الممنوع: هل اكتسب التطبيق لديك رمزًا مميزًا لمطابقة الأذونات المختارة؟**

تأكد من أن أنواع الأذونات المطلوبة أو الممنوحة تطابق نوع رمز الوصول الذي يكتسبه تطبيقك. قد تطلب أذونات التطبيق وتمنحها ولكن تستخدم الرموز المميزة لتدفق التعليمات البرمجية التفاعلية المفوضة بدلاً من الرموز المميزة لتدفق بيانات اعتماد العميل، أو تطلب الأذونات المفوضة ومنحها ولكن باستخدام رموز تدفق بيانات اعتماد العميل بدلاً من الرموز المميزة لتدفق التعليمات البرمجية المفوضة.

لمزيد من المعلومات المتعلقة بالحصول على الرموز المميزة، راجع:

- [الحصول على حق الوصول نيابة عن المستخدمين والأذونات المفوضة](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 - تدفق كود تفويض OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [احصل على حق الوصول بدون مستخدم (خدمة خفية) وأذونات التطبيق](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 - تدفق بيانات اعتماد عميل OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**خطأ الحظر 403: إعادة تعيين كلمة المرور**

حاليًا، لا توجد أذونات خفيّة لإذن التطبيق تسمح بإعادة تعيين كلمات مرور المستخدم. يتم دعم واجهات برمجة التطبيقات هذه فقط باستخدام تدفقات التعليمات البرمجية المفوضة التفاعلية مع مسؤول مسجل الدخول. لمزيد من المعلومات، راجع [أذونات Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**حظر 403: هل لدى المستخدم حق الوصول وهل هو مرخص؟**

بالنسبة لتدفقات الرمز المفوض، يقوم Microsoft Graph بتقييم ما إذا كان قد تم السماح بالطلب بناءً على الأذونات الممنوحة للتطبيق، والأذونات التي يمتلكها المستخدم الذي قام بتسجيل الدخول. بشكل عام، يشير هذا الخطأ إلى أن المستخدم ليس لديه امتيازات كافية لتنفيذ الطلب **أو** أن المستخدم غير مرخص له للبيانات التي يتم الوصول إليها. يمكن فقط للمستخدمين الذين لديهم الأذونات، أو التراخيص المطلوبة تقديم الطلب بنجاح.

**حظر 403: هل حددت API المورد الصحيح؟**

تفحص خدمات API مثل Microsoft Graph من أن المطالبة بـ *aud* (الجمهور) في رمز الوصول المميز الذي تم تلقيه تطابق القيمة المتوقعة لنفسه، وإذا لم يكن الأمر كذلك، يحدث خطأ حظر 403. هناك خطأ شائع ينتج عن هذا الخطأ وهو محاولة استخدام رمز مميز تم الحصول عليه لـ API لـ Azure AD Graph أو API لـ Outlook أو API لـ SharePoint / OneDrive للاتصال بـ Microsoft Graph (أو العكس). تأكد من أن المورد (أو النطاق) يكتسب تطبيقك رمزًا مميزًا بمرات التطابق مع API التي يستدعيها التطبيق.

**الطلب السيئ لـ 400 أو المحظور 403: هل يلتزم المستخدم بسياسات الوصول المشروط (CA) للمؤسسة؟**

استنادًا إلى سياسات الوصول المشروط (CA) للمؤسسة، قد يتم تحدي المستخدم الذي يصل إلى موارد Microsoft Graph عبر التطبيق الخاص بك للحصول على معلومات إضافية غير موجودة في رمز الوصول الذي حصل عليه تطبيقك في الأصل. في هذه الحالة، يتلقى تطبيقك **400 بخطأ *interaction_required*** أثناء الحصول على رمز الوصول المميز أو **403 مع *insufficient_claims*** عند الاتصال بـ Microsoft Graph. في كلتا الحالتين، تحتوي استجابة الخطأ على معلومات إضافية يمكن تقديمها إلى نقطة النهاية المصرح بها لتحدي المستخدم للحصول على معلومات إضافية (مثل المصادقة متعددة العوامل، أو تسجيل الجهاز).

لمزيد من المعلومات المتعلقة بالوصول المشروط، راجع:

- [التعامل مع تحديات الوصول المشروط باستخدام MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [إرشادات المطور للوصول المشروط إلى Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_إنهاء دعم مكتبة مصادقة Azure Active Directory (ADAL) و Azure AD Graph API (AAD Graph)_* _

- اعتبارًا من 30 يونيو 2020، لن نضيف أي ميزات جديدة إلى مكتبة مصادقة Azure Active Directory (ADAL) وAPI لـ Azure AD Graph (AAD Graph). سنستمر في تقديم الدعم الفني وتحديثات الأمان ولكننا لن نقدم تحديثات للميزات بعد الآن.
- اعتبارًا من 30 يونيو 2022، سننهي دعم ADAL وAAD Graph، ولن نقدم بعد الآن دعمًا فنيًا أو تحديثات الأمان.
    - ستستمر التطبيقات التي تستخدم ADAL على إصدارات نظام التشغيل الحالية في العمل بعد هذا الوقت ولكنها لن تحصل على أي دعم فني أو تحديثات الأمان.
    - قد لا تتلقى التطبيقات التي تستخدم AAD Graph بعد هذا الوقت استجابات من نقطة نهاية AAD Graph.

_ *ترحيل ADAL**

نوصي بالتحديث إلى [مكتبة مصادقة Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)، التي تحتوي على أحدث الميزات وتحديثات الأمان. تأتي هذه التوصية في سياق ترحيل Microsoft لتطبيقاتها إلى MSAL بحلول الموعد النهائي لنهاية الدعم. الهدف من ترحيل تطبيقات Microsoft إلى MSAL هو ضمان استفادة التطبيقات من التحسينات المستمرة للأمان والميزات في MSAL.

- [قراءة الأسئلة الشائعة حول ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [تعرّف على كيفية ترحيل التطبيقات على أساس كل نظام أساسي](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- إذا كنت بحاجة إلى مساعدة في فهم أي من تطبيقاتك تستخدم ADAL، فإننا نوصيك بتقييم جميع التعليمات البرمجية المصدر لتطبيقاتك، وإذا أمكن، يمكنك التواصل مع أي من موردي البرامج المستقلين (ISV) أو موفري التطبيقات. يمكن أن يوفر لك دعم Microsoft أيضًا قائمة بجميع تطبيقات ADAL غير التابعة لـ Microsoft في المستأجر الخاص بك.

**ترحيل AAD Graph**

للتطبيقات التي تستخدم AAD Graph، اتبع إرشاداتنا [لترحيل تطبيقات Azure AD Graph إلى Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [توفر قائمة اختيار الترحيل نقطة بدء استخدام](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- يُُظهر مدخل تسجيل تطبيق Azure التطبيقات التي تستخدم AAD Graph. نوصيك بمراجعة جميع التعليمات البرمجية المصدر لتطبيقاتك، وإذا أمكن، يمكنك الوصول إلى أي من موردي البرامج المستقلين أو مزودي التطبيقات. يمكن أن يوفر لك دعم Microsoft أيضا معلومات حول استخدام AAD Graph لدى المستأجر.

 










