---
title: الاستعلام عن واجهه برمجه تطبيقات Microsoft Graph
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
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974151"
---
# <a name="querying-the-microsoft-graph-api"></a>الاستعلام عن واجهه برمجه تطبيقات Microsoft Graph

قد ينطبق هذا الموضوع أيضا علي المطورين الذين لا يزالوا يستخدمون واجهه برمجه تطبيقات Azure AD. ومع ذلك ، يوصي **بشده** باستخدام Microsoft Graph لكل الدليل والهوية وسيناريوهات أداره access.

**مشاكل المصادقة أو التخويل**

- إذا تعذر علي تطبيقك **الحصول علي الرموز المميزة** للاتصال ب microsoft graph ، فاختر **المشكلة المتعلقة بالحصول علي التعليمات الخاصة بالرمز المميز للوصول (مصادقه)** microsoft Graph للحصول علي مزيد من المساعدة والدعم في هذا الموضوع.
- إذا كان التطبيق الذي تريده **يتلقى 401 أو 403 خطا في التخويل** عند الاتصال بالرسم البياني ل microsoft ، فحدد الفئة الخاصة **بالحصول علي الأخطاء التي رفضها Access (التخويل)** للحصول علي تعليمات ودعم أكثر تحديدا في هذا الموضوع.

**ارغب في استخدام Microsoft Graph ، ولكن ليس عليك التاكد من مكان البدء**

لمعرفه المزيد حول Microsoft Graph ، راجع:

- [نظره عامه حول Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [نظره عامه حول الهوية وأداره Access في Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [بدء إنشاء تطبيقات Microsoft Graph](https://docs.microsoft.com/graph/)
- **مستكشف الرسوم البيانية في microsoft** -اختبار واجات برمجه تطبيقات microsoft graph في نطاق المستاجر أو مستاجر العرض التوضيحي

**أريد استخدام Microsoft Graph ، ولكنه يدعم الدليل v 1.0 واجات برمجه التطبيقات التي احتاج اليها ؟**

ان Microsoft Graph هو واجهه برمجه التطبيقات الموصي بها للدليل والهوية وأداره الوصول. ومع ذلك ، لا تزال هناك بعض الفجوات بين العناصر الممكنة في Azure AD Graph و Microsoft Graph. راجع المقالات التالية التي تميز معظم الاختلافات المحدثة للمساعدة في اختيارك:

- [اختلافات أنواع الموارد بين الرسم البياني ل Azure AD و Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [اختلافات الخصائص بين الرسم البياني ل Azure AD و Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [اختلافات الأسلوب بين Azure AD و Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**عند الاستعلام عن عنصر *المستخدم* ، تكون العديد من خصائصه مفقوده**

`GET https://graph.microsoft.com/v1.0/users` تقوم فقط بإرجاع الخاصية 11 ، بما في ذلك Microsoft Graph يحدد تلقائيا مجموعه افتراضيه من خصائص *المستخدم* لإرجاعها. إذا كنت بحاجه إلى خصائص *مستخدم* أخرى ، فاستخدم $select لاختيار الخصائص التي يحتاج اليها التطبيق. جربه في **Microsoft Graph Explorer** أولا.

**بعض قيم خصائص المستخدم *فارغه* علي الرغم من انه اعلم انه تم تعيينها**

التوضيح الأكثر احتمالا هو انه تم منح التطبيق *ريدباسيك* . يتيح هذا للتطبيق قراءه مجموعه محدوده من خصائص المستخدم ، وإرجاع كل الخصائص الأخرى كفارغه حتى إذا تم تعيينها مسبقا. جرب منح *المستخدم التطبيق. أقرا كل* الأذونات بدلا من ذلك.

لمزيد من المعلومات ، راجع [أذونات مستخدمي Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**أواجه مشكله في استخدام معلمات استعلام OData لتصفيه البيانات في طلباتي**

بينما يدعم Microsoft Graph مجموعه كبيره من معلمات الاستعلام OData ، لا يتم دعم العديد من هذه المعلمات بشكل كامل بواسطة خدمات الدليل (الموارد التي ترث من *ديريكتوريوبجيكت*) في Microsoft Graph. تستمر القيود نفسها التي كانت موجودة في الرسم البياني في Azure AD

1. **غير معتمد**: $count و $search و $filter علي قيم *خاليه* أو *فارغه*
2. **غير معتمد**: $filter علي خصائص معينه (راجع مواضيع الموارد التي يتم قابله للتصفية الخصائص بها)
3. **غير معتمد**: الترحيل والتصفية والفرز في الوقت نفسه
4. **غير معتمد**: تصفيه علاقة. علي سبيل المثال ، يمكنك العثور علي كل أعضاء المجموعة الهندسية الموجودة في المملكة المتحدة.
5. **الدعم الجزئي**: $orderby علي *المستخدم* (displayName و الوحدات التي ليست فقط) والمجموعة 
6. **الدعم الجزئي**: $filter ( *يعتمد فقط* الدعم *الستارتسويث* أو الدالات الفردية *أو* المحدودة) ، وال$expand (توسيع علاقات كائن واحد ترجع كل العلاقات ، ولكن توسيع مجموعه من الكائنات التي تقتصر عليها العلاقات) 

لمزيد من المعلومات ، راجع [تخصيص الاستجابات باستخدام معلمات الاستعلام](https://docs.microsoft.com/graph/query-parameters).

**لا تعمل واجهه برمجه التطبيقات (API) التي أقوم بالاتصال بها ، حيث يمكنني اجراء المزيد من الاختبارات ؟**

**مستكشف Microsoft graph** -اختبر واجات برمجه تطبيقات microsoft graph في نطاق المستاجر أو مستاجر العرض التوضيحي ، وراجع أيضا **نماذج الاستعلامات** في مستكشف Microsoft Graph.

**عندما أقوم بالاستعلام عن بيانات يبدو انه تمت أعاده تعيين بيانات غير مكتملة**

إذا كنت تقوم بالاستعلام عن مجموعه (مثل *المستخدمين*) ، فان Microsoft Graph يستخدم حدود الصفحة من جانب الخادم حتى يتم دائما إرجاع النتائج بحجم صفحه افتراضي. يجب ان يتوقع تطبيقك دائما الوصول إلى الصفحة عبر المجموعات التي يتم إرجاعها من الخدمة.

لمزيد من المعلومات، اطلع على:

- [أفضل الممارسات في Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [ترحيل بيانات الرسومات البيانية في Microsoft إلى التطبيق](https://docs.microsoft.com/graph/paging)

**التطبيق الخاص بي بطيء جدا وهو أيضا يتم التحكم فيه. ما هي التحسينات التي يمكنني القيام بها ؟**

استنادا إلى السيناريو الذي تستخدمه ، هناك مجموعه متنوعة من الخيارات المختلفة عند التخلص لتطبيقك بشكل أكثر فاعليه ، وفي بعض الحالات ، اقل عرضه ليتم التحكم فيها من قبل الخدمة (عند اجراء مكالمات كثيره جدا).

للتعرّف على المزيد، اطلع على:

- [أفضل الممارسات في Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [طلبات التجميع](https://docs.microsoft.com/graph/json-batching)
- [تعقب التغييرات عبر استعلام دلتا](https://docs.microsoft.com/graph/delta-query-overview)
- [الحصول علي اعلام بالتغييرات عبر ويبهوكس](https://docs.microsoft.com/graph/webhooks)
- [إرشادات التحكم](https://docs.microsoft.com/graph/throttling)

**أين يمكنني العثور علي مزيد من المعلومات حول الأخطاء والمشاكل المعروفة ؟**

- [معلومات الاستجابة لخطا Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [المشاكل المعروفة في Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**أين يمكنني التحقق من حاله توفر الخدمة والاتصال ؟**

يمكن ان تؤثر أتاحه الخدمة والاتصال بالخدمات الاساسيه التي يمكن الوصول اليها من خلال Microsoft Graph علي التوفر والأداء الكلي ل Microsoft Graph.

- بالنسبة إلى حماية خدمه Active Directory في Azure ، تحقق من حاله **الأمان + خدمات الهوية** المدرجة في [صفحه حاله Azure](https://azure.microsoft.com/status/).
- بالنسبة إلى خدمات Office التي تساهم في Microsoft Graph ، تحقق من حاله الخدمات المدرجة في [لوحه معلومات حماية خدمه Office](https://portal.office.com/adminportal/home#/servicehealth).
