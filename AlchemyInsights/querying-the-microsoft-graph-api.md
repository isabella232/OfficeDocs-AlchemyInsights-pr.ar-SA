---
title: الاستعلام عن Microsoft Graph API
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
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923226"
---
# <a name="querying-the-microsoft-graph-api"></a>الاستعلام عن Microsoft Graph API

قد ينطبق هذا الموضوع أيضا على المطورين الذين ما زالوا يستخدمون Azure AD Graph API. ومع **ذلك،** يوصى بشدة باستخدام microsoft Graph لكل سيناريوهات إدارة الدليل والهوية والوصول.

**مشاكل المصادقة أو التفويض**

- إذا تعذر  على تطبيقك الحصول على الرموز المميزة لاستدعاء Microsoft Graph، فاختار مشكلة في الحصول على رمز وصول **مميز (مصادقة)** فئة Microsoft Graph للحصول على تعليمات ودعم أكثر تحديدا حول هذا الموضوع.
- إذا كان التطبيق يتلقى **أخطاء تخويل 401 أو 403** عند الاتصال ب Microsoft Graph، فاختار الفئة الحصول على خطأ رفض الوصول **(تخويل)** Microsoft Graph API للحصول على تعليمات ودعم أكثر تحديدا حول هذا الموضوع.

**أريد استخدام Microsoft Graph، ولكن لست متأكدا من مكان البدء**

لمعرفة المزيد حول Microsoft Graph، راجع:

- [نظرة عامة على Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [نظرة عامة حول إدارة الهوية والوصول في Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [بدء إنشاء تطبيقات Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - اختبار واجهات برمجة تطبيقات Microsoft Graph في المستأجر أو مستأجر عرض توضيحي

**أريد استخدام Microsoft Graph، ولكن هل يدعم واجهات برمجة تطبيقات الدليل التي أحتاج إليها في v1.0؟**

Microsoft Graph هي API المستحسنة لإدارة الدليل والهوية والوصول. ومع ذلك، لا تزال هناك بعض الثغرات بين ما هو ممكن في Azure AD Graph و Microsoft Graph. راجع المقالات التالية، التي تسلط الضوء على أحدث الاختلافات لمساعدتك في اختيارك:

- [اختلافات نوع المورد بين Azure AD Graph و Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [اختلافات في الممتلكات بين Azure AD Graph و Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [اختلافات الأسلوب بين Azure AD و Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**عند الاستعلام عن *كائن* المستخدم، تكون العديد من خصائصه مفقودة**

`GET https://graph.microsoft.com/v1.0/users`ترجع فقط 11 من الخصائص، بينما تقوم Microsoft Graph تلقائيا بتحديد مجموعة افتراضية من *خصائص* المستخدم التي سيتم إرجاعها. إذا كنت بحاجة إلى *خصائص مستخدم* أخرى، فاستخدم $select لاختيار الخصائص التي يحتاج إليها التطبيق. جرب ذلك في **Microsoft Graph Explorer** أولا.

**بعض قيم خاصية المستخدم *فارغة* على الرغم من أنني أعرف أنها تم تعيينها**

التفسير الأكثر شيوعا هو أنه تم منح التطبيق الإذن *User.ReadBasic.All.* يسمح هذا للتطبيق بقراءة مجموعة محدودة من خصائص المستخدم، مع إرجاع كل الخصائص الأخرى ك خالية حتى لو تم تعيينها مسبقا. حاول منح التطبيق *إذن User.Read.All* بدلا من ذلك.

لمزيد من المعلومات، راجع [أذونات Graph Microsoft](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**أواجه مشكلة في استخدام معلمات استعلام OData لتصفية البيانات في طلباتي**

على الرغم Graph Microsoft يدعم مجموعة واسعة من معلمات استعلام OData، فإن خدمات الدليل (الموارد التي ترث من *الدليلObject)* غير معتمدة بشكل كامل في Microsoft Graph. تستمر القيود نفسها التي كانت موجودة في Azure AD Graph في Microsoft Graph:

1. **غير معتمد**: $count $search وقيم $filter قيم *خالية* أو *غير* خالية
2. **غير معتمد**: $filter خصائص معينة (راجع مواضيع الموارد التي يمكن تصفيتها)
3. **غير معتمد**: الترحيل والتصفية والفرز في الوقت نفسه
4. **غير معتمد**: التصفية على علاقة. على سبيل المثال - ابحث عن كل أعضاء المجموعة الهندسية في المملكة المتحدة.
5. **دعم جزئي**: $orderby *المستخدم* (displayName و userPrincipalName فقط) *والمجموعة*
6. **دعم** جزئي: $filter (يدعم فقط *eq* وبداية مع و محدود أي *دعم)،* فإن $expand (توسيع علاقات كائن واحد يرجع كل العلاقات، ولكن توسيع مجموعة من علاقات الكائنات محدود)  

لمزيد من المعلومات، راجع [تخصيص الاستجابات باستخدام معلمات الاستعلام](https://docs.microsoft.com/graph/query-parameters).

**لا تعمل API التي أقوم بالاتصال بها - أين يمكنني إجراء المزيد من الاختبارات؟**

**Microsoft Graph Explorer** - اختبر واجهات برمجة تطبيقات Microsoft Graph في المستأجر أو  المستأجر التجريبي وافحص أيضا الاستعلامات العينة في Microsoft Graph Explorer.

**عندما أستعلام عن البيانات، يبدو أنني أستعيد مجموعة بيانات غير مكتملة**

إذا كنت تقوم باستعلام مجموعة (مثل المستخدمين)، Graph Microsoft حدود الصفحات من جانب الخادم بحيث يتم دائما إرجاع النتائج بحجم صفحة افتراضي. يجب أن يتوقع تطبيقك دائما عرض الصفحات عبر المجموعات التي يتم إرجاعها من الخدمة.

لمزيد من المعلومات، اطلع على:

- [أفضل Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [ترحيل بيانات Microsoft Graph في تطبيقك](https://docs.microsoft.com/graph/paging)

**تطبيقي بطيء جدا، كما أنه يتم أيضا كبحه. ما هي التحسينات التي يمكنني إدخالها؟**

وفقا للسيناريو الخاص بك، هناك مجموعة متنوعة من الخيارات المختلفة تحت تصرفك لجعل تطبيقك أكثر أداء، وفي بعض الحالات، أقل عرضة للتوقف عن الخدمة (عندما تقوم بإجراء عدد كبير جدا من المكالمات).

للتعرّف على المزيد، اطلع على:

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
