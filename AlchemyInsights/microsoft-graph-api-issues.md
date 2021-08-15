---
title: مشاكل Graph API ل Microsoft
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
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975880"
---
# <a name="microsoft-graph-api-issues"></a>مشاكل Graph API ل Microsoft

قد ينطبق هذا الموضوع أيضا على المطورين الذين ما زالوا يستخدمون Azure AD Graph API. ومع **ذلك،** يوصى بشدة باستخدام microsoft Graph لكل سيناريوهات إدارة الدليل والهوية والوصول.

**مشاكل المصادقة أو التفويض**

- إذا تعذر  على تطبيقك الحصول على الرموز المميزة لاستدعاء Microsoft Graph، فاختار مشكلة في الحصول على رمز وصول **مميز (مصادقة)** فئة Microsoft Graph للحصول على تعليمات ودعم أكثر تحديدا حول هذا الموضوع.
- إذا كان التطبيق يتلقى **أخطاء تخويل 401 أو 403** عند الاتصال ب Microsoft Graph، فاختار الفئة الحصول على خطأ رفض الوصول **(تخويل)** Microsoft Graph API للحصول على تعليمات ودعم أكثر تحديدا حول هذا الموضوع.

**أريد استخدام Microsoft Graph، ولكن لست متأكدا من مكان البدء**

- [نظرة عامة على Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [نظرة عامة حول إدارة الهوية والوصول في Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [بدء إنشاء تطبيقات Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - اختبار واجهات برمجة تطبيقات Microsoft Graph في المستأجر أو مستأجر عرض توضيحي

**أريد استخدام Microsoft Graph، ولكن هل يدعم واجهات برمجة تطبيقات الدليل التي أحتاج إليها في v1.0؟**

Microsoft Graph هي API المستحسنة لإدارة الدليل والهوية والوصول. ومع ذلك، لا تزال هناك بعض الثغرات بين ما هو ممكن في Azure AD Graph و Microsoft Graph. راجع المقالات التالية، التي تسلط الضوء على أحدث الاختلافات لمساعدتك في اختيارك:

- [اختلافات نوع المورد بين Azure AD Graph و Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [اختلافات في الممتلكات بين Azure AD Graph و Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [اختلافات الأسلوب بين Azure AD و Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**لا تعمل API التي أقوم بالاتصال بها - أين يمكنني إجراء المزيد من الاختبارات؟**

**Microsoft Graph Explorer** - اختبر واجهات برمجة تطبيقات Microsoft Graph في المستأجر أو  المستأجر التجريبي وافحص أيضا الاستعلامات العينة في Microsoft Graph Explorer.

**تطبيقي بطيء جدا، كما أنه يتم أيضا كبحه. ما هي التحسينات التي يمكنني إدخالها؟**

وفقا للسيناريو الخاص بك، هناك مجموعة متنوعة من الخيارات تحت تصرفك لجعل تطبيقك أكثر أداء، وفي بعض الحالات، أقل عرضة للتوقف عن الخدمة (عندما تقوم بإجراء مكالمات كثيرة جدا).

- [أفضل Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [طلبات الدفع](https://docs.microsoft.com/graph/json-batching)
- [تعقب التغييرات من خلال استعلام دلتا](https://docs.microsoft.com/graph/delta-query-overview)
- [الحصول على إعلام بالتغييرات من خلال webhooks](https://docs.microsoft.com/graph/webhooks)
- [إرشادات الوتد](https://docs.microsoft.com/graph/throttling)

**أين يمكنني العثور على مزيد من المعلومات حول الأخطاء والقضايا المعروفة؟**

- [معلومات استجابة Graph Microsoft](https://docs.microsoft.com/graph/errors)
- [المشاكل المعروفة في Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**أين يمكنني التحقق من حالة توفر الخدمة واتصالها؟**

يمكن أن يؤثر توفر الخدمة واتصال الخدمات الأساسية التي يمكن الوصول إليها عبر Microsoft Graph على التوفر والأداء العامين لخدمات Microsoft Graph.

- للحصول على حماية خدمة Azure Active Directory، تحقق من حالة **خدمات الأمان +** الهوية المدرجة في صفحة حالة [Azure](https://azure.microsoft.com/status/).
- بالنسبة Office الخدمات التي تساهم في Microsoft Graph، تحقق من حالة الخدمات المدرجة في لوحة Office [حالة الخدمة.](https://portal.office.com/adminportal/home#/servicehealth)

قد Graph أخطاء التخويل من Microsoft نتيجة لعدة مشاكل مختلفة، معظمها يؤدي إلى حدوث خطأ 401 أو 403. على سبيل المثال، يمكن أن يؤدي كل ما يلي إلى حدوث أخطاء التخويل:

- [تدفقات الحصول على الرمز المميز للوصول](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios) غير صحيحة
- [نطاقات الأذونات](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) تم تكوينها بشكل غير صحيح
- عدم [الموافقة](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***انتهاء الدعم لمكتبة مصادقة Azure Active Directory (ADAL) و Azure AD Graph API (AAD Graph)***

**بدءا من 30 يونيو 2020،** لن نضيف أي ميزات جديدة إلى ADAL و Azure AD Graph. سنستمر في تقديم الدعم الفني وتحديثات الأمان ولكننا لن نقدم تحديثات للميزات بعد الآن.

**بدءا من 30 يونيو 2022،** سننهي دعم ADAL و Azure AD Graph ولن نوفر تحديثات الأمان أو الدعم التقني.

ستستمر التطبيقات التي تستخدم ADAL على إصدارات نظام التشغيل الموجودة في العمل بعد هذا الوقت ولكنها لن تحصل على أي تحديثات أمنية أو *دعم تقني.*

قد لا تتلقى التطبيقات التي تستخدم Azure AD Graph بعد هذا الوقت استجابات من نقطة نهاية Azure AD Graph نهاية.

**ترحيل ADAL**

نوصي بالتحديث إلى [مكتبة مصادقة Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)، التي تحتوي على أحدث الميزات وتحديثات الأمان.

إذا كنت تستخدم تطبيقات Microsoft، فتعرف على أن Microsoft تقوم بتهجر تطبيقاتها إلى MSAL بحلول الموعد النهائي لنهاية الدعم، مع التأكد من أنها ستستفيد من تحسينات الميزات والأمان المستمرة ل MSAL.

1. [قراءة الأسئلة الشائعة حول ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [تعرّف على كيفية ترحيل التطبيقات على أساس كل نظام أساسي](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. إذا كنت بحاجة إلى مساعدة في فهم التطبيقات التي تستخدم ADAL، فإننا ننصحك بمراجعة التعليمات البرمجية المصدر لتطبيقاتك، وإذا كان ذلك قابلا للتطبيق، فصل إلى أي موفري خدمات الإنترنت أو موفري التطبيقات. يمكن أن يوفر لك دعم Microsoft أيضًا قائمة بجميع تطبيقات ADAL غير التابعة لـ Microsoft في المستأجر الخاص بك.

**ترحيل AAD Graph**

بالنسبة للتطبيقات التي تستخدم Azure AD Graph، اتبع إرشاداتنا لترحيل [تطبيقات Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)إلى Microsoft Graph .

1. [توفر قائمة اختيار الترحيل نقطة بدء استخدام](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. يُُظهر مدخل تسجيل تطبيق Azure التطبيقات التي تستخدم AAD Graph. نوصيك بمراجعة جميع التعليمات البرمجية المصدر لتطبيقاتك، وإذا أمكن، يمكنك الوصول إلى أي من موردي البرامج المستقلين أو مزودي التطبيقات. يمكن أن يوفر لك دعم Microsoft أيضا قائمة بكل برامج AAD Graph في المستأجر.
3. لكي يمكن لتطبيقك الوصول إلى البيانات في Microsoft Graph، يجب على المستخدم أو المسؤول منحه الأذونات الصحيحة عبر عملية موافقة. يسرد [مرجع Graph](https://docs.microsoft.com/graph/permissions-reference) Microsoft الأذونات المقترنة بكل مجموعة رئيسية من واجهات برمجة التطبيقات Graph Microsoft. كما يوفر إرشادات حول كيفية استخدام الأذونات.
