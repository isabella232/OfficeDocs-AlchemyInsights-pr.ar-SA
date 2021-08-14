---
title: أخطاء التطبيق
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931436"
---
# <a name="application-errors"></a>أخطاء التطبيق

هل تبحث عن معلومات حول رموز **الخطأ AADSTS** التي يتم إرجاعها من خدمة الرمز المميز ل Azure Active Directory (Azure AD)؟ اقرأ [رموز أخطاء مصادقة Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) والتخويل للعثور على أوصاف أخطاء AADSTS وإصلاحاتها وبعض الحلول المقترحة.

يمكن أن تكون أخطاء التخويل نتيجة للعديد من المشكلات المختلفة، والتي ينتج عن معظمها خطأ 401 أو 403. على سبيل المثال، يمكن أن يؤدي كل ما يلي إلى حدوث أخطاء التخويل:

- [تدفقات الحصول على الرمز المميز للوصول](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) غير صحيحة 
- [نطاقات الأذونات](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) تم تكوينها بشكل غير صحيح 
- عدم [الموافقة](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

لحل أخطاء التخويل الشائعة، جرب الخطوات المذكورة أدناه الأكثر تطابقا للخطأ الذي تستلمه. قد ينطبق أكثر من واحد.

**401 خطأ غير مخوّل: هل رمزك المميز صالح؟**

تأكد من أن تطبيقك يقدم رمز وصول مميز صالحا Graph Microsoft كجزء من الطلب. غالبًا ما يعني هذا الخطأ أن رمز الوصول قد يكون مفقودًا في رأس صفحة طلب مصادقة HTTP أو أن الرمز المميز غير صالح أو انتهت صلاحيته. نوصي بشدة باستخدام [مكتبة مصادقة Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) للحصول على رمز الوصول المميز. بالإضافة إلى ذلك، قد يحدث هذا الخطأ إذا حاولت استخدام رمز وصول مميز مفوض تم منحه إلى حساب Microsoft شخصي للوصول إلى API الذي يدعم فقط حسابات العمل أو المؤسسة (حسابات المؤسسة).

**403 خطأ ممنوع: هل اخترت المجموعة المناسبة من الأذونات؟**

تحقق من أنك طلبت مجموعة الأذونات الصحيحة استنادا إلى أذونات Microsoft Graph واجهات برمجة التطبيقات التي يتصل بها تطبيقك. يتم توفير أقل الأذونات المميزة المستحسنة في كل مواضيع أسلوب مرجع Graph API ل Microsoft. بالإضافة إلى ذلك، يجب أن يتم منح تلك الأذونات للتطبيق من قبل مستخدم أو مسؤول. يتم منح الأذونات عادة من خلال صفحة موافقة أو من خلال منح الأذونات باستخدام شفرة تسجيل تطبيق Azure Portal. من شفرة **الإعدادات** للتطبيق، انقر فوق **الأذونات المطلوبة**، ثم انقر فوق **منح الأذونات**.

- [أذونات Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [فهم أذونات Azure AD والموافقة عليها](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**الخطأ 403 الممنوع: هل اكتسب التطبيق لديك رمزًا مميزًا لمطابقة الأذونات المختارة؟**

تأكد من أن نوع الأذونات المطلوبة أو الممنوحة يتطابق مع نوع رمز الوصول المميز الذي يحصل عليه تطبيقك. قد تطلب أذونات التطبيق وتمنحها ولكنك تستخدم الرموز المميزة لتدفق التعليمات البرمجية التفاعلية المفوضة بدلا من الرموز المميزة لتدفق بيانات الاعتماد للعميل، أو تطلب الأذونات المفوضة وتمنحها ولكن باستخدام الرموز المميزة لتدفق بيانات اعتماد العميل بدلا من الرموز المميزة لتدفق التعليمات البرمجية المفوضة.

- [الحصول على حق الوصول نيابة عن المستخدمين والأذونات المفوضة](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - تدفق كود تفويض OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [احصل على حق الوصول بدون مستخدم (خدمة خفية) وأذونات التطبيق](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - تدفق بيانات اعتماد عميل OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**خطأ الحظر 403: إعادة تعيين كلمة المرور**

حاليًا، لا توجد أذونات خفيّة لإذن التطبيق تسمح بإعادة تعيين كلمات مرور المستخدم. يتم دعم واجهات برمجة التطبيقات هذه فقط باستخدام تدفقات التعليمات البرمجية المفوضة التفاعلية مع مسؤول مسجل الدخول.

- [أذونات Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**حظر 403: هل لدى المستخدم حق الوصول وهل هو مرخص؟**

بالنسبة لتدفقات التعليمات البرمجية المفوضة، يتم تقييم Graph Microsoft إذا كان الطلب مسموحا به استنادا إلى الأذونات الممنوحة للتطبيق والأذونات التي لدى المستخدم الذي قام تسجيل الدخول. بشكل عام، يشير هذا الخطأ إلى أن المستخدم ليس لديه امتيازات كافية لتنفيذ الطلب أو  أن المستخدم غير مرخص له للبيانات التي يتم الوصول إليها. يمكن فقط للمستخدمين الذين لديهم الأذونات، أو التراخيص المطلوبة تقديم الطلب بنجاح.

**حظر 403: هل حددت API المورد الصحيح؟**

تحقق خدمات API مثل Microsoft Graph من تطابق المطالبة بالعلامة aud (الجمهور) في رمز الوصول المميز الذي تم تلقيه مع القيمة التي يتوقعها لنفسه، وإذا لم يكن الأمر كذلك، فإنه ينتج عنه خطأ 403 ممنوع. هناك خطأ شائع ينتج عن هذا الخطأ وهو محاولة استخدام رمز مميز تم الحصول عليه لـ API لـ Azure AD Graph أو API لـ Outlook أو API لـ SharePoint / OneDrive للاتصال بـ Microsoft Graph (أو العكس). تأكد من أن المورد (أو النطاق) يكتسب تطبيقك رمزًا مميزًا بمرات التطابق مع API التي يستدعيها التطبيق.

**الطلب السيئ لـ 400 أو المحظور 403: هل يلتزم المستخدم بسياسات الوصول المشروط (CA) للمؤسسة؟**

استنادا إلى سياسات CA الخاصة ب المؤسسة، قد يتم تحدي مستخدم يقوم بالوصول إلى موارد Microsoft Graph عبر تطبيقك للحصول على معلومات إضافية غير موجودة في رمز الوصول المميز الذي حصل عليه تطبيقك في الأصل. في هذه الحالة، يتلقى تطبيقك 400 بخطأ *interaction_required* أثناء الحصول على رمز الوصول المميز أو 403 مع *insufficient_claims* عند الاتصال بـ Microsoft Graph. في كلتا الحالتين، تحتوي استجابة الخطأ على معلومات إضافية يمكن تقديمها إلى نقطة النهاية تخويل لتحدي المستخدم للحصول على معلومات إضافية (مثل المصادقة متعددة العوامل أو تسجيل الجهاز).

- [معالجة تحديات الوصول الشرطي باستخدام MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [إرشادات المطور للوصول المشروط إلى Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
