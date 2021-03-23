---
title: استخدام مكتبات المصادقة
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034754"
---
# <a name="working-with-authentication-libraries"></a>استخدام مكتبات المصادقة

لحل مشكلة مكتبة مصادقة Microsoft (MSAL)، يجب تنفيذ الخطوات الموصى بها التالية:

1. **استخدام MSAL**: [مكتبات](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) مصادقة النظام الأساسي لهوية Microsoft - تعرض هذه المقالة دعم مكتبة مصادقة Microsoft لأنواع تطبيقات متعددة. ويتضمن ارتباطات إلى التعليمات البرمجية المصدر للمكتبة؛ مكان الحصول على حزمة لمشروع تطبيقك؛ وما إذا كانت المكتبة تدعم تسجيل دخول المستخدم (المصادقة) أو الوصول إلى واجهات برمجة تطبيقات الويب المحمية (التخويل) أو كليهما.

2. **استكشاف الأخطاء وإصلاحها المصادقة**: تدعم MSAL العديد من تدفقات المصادقة لاستخدامها في سيناريوهات تطبيق مختلفة. استنادا إلى كيفية إنشاء تطبيق العميل، يمكن ل MSAL استخدام واحد أو أكثر من تدفقات المصادقة المعتمدة من النظام الأساسي لهوية Microsoft. يمكن لهذه التدفقات أن تنتج أنواعا متعددة من الرموز المميزة ورموز التخويل، وتتطلب رموزا مميزا مختلفة لجعلها تعمل.

3. **رموز Access** المميزة : الرموز المميزة للوصول إلى النظام الأساسي لهوية [Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - تعرف على كيفية التحقق من صحة API واستخدام المطالبات داخل رمز الوصول المميز. تنطبق كل الوثائق في هذه المقالة، باستثناء الوثائق التي تم ذكرها، فقط على الرموز المميزة التي تم إصدارها ل واجهات برمجة التطبيقات التي قمت بتسجيلها. ولا ينطبق على الرموز المميزة التي تم إصدارها ل واجهات برمجة التطبيقات المملوكة ل Microsoft، ولا يمكن استخدام هذه الرموز المميزة للتحقق من كيفية إصدار النظام الأساسي لهوية Microsoft الرموز المميزة ل API التي تقوم بإنشاءها.

**انتهاء الدعم لمكتبة مصادقة Azure Active Directory (ADAL)**

- **اعتبارا من 30 يونيو 2020،** لن نضيف أي ميزات جديدة إلى ADAL و Azure AD Graph. سنستمر في تقديم الدعم الفني وتحديثات الأمان ولكننا لن نقدم تحديثات للميزات بعد الآن.
- **اعتبارا من 30 يونيو 2022،** سننهي دعم ADAL و Azure AD Graph ولن نوفر تحديثات الأمان أو الدعم التقني.
- ستستمر التطبيقات التي تستخدم ADAL على إصدارات نظام التشغيل الموجودة في العمل بعد هذا الوقت ولكنها لن تحصل على أي تحديثات أمنية أو *دعم تقني.*
- قد لا تتلقى التطبيقات التي تستخدم Azure AD Graph بعد هذا الوقت استجابات من نقطة نهاية Azure AD Graph.

**ترحيل ADAL**

- نوصي بالتحديث إلى MSAL، الذي يضم أحدث الميزات وتحديثات الأمان.
- إذا كنت تستخدم تطبيقات Microsoft، فتعرف على أن Microsoft تقوم بتهجر تطبيقاتها إلى MSAL بحلول الموعد النهائي لنهاية الدعم، مع التأكد من أنها ستستفيد من تحسينات الميزات والأمان المستمرة ل MSAL.

1. [اقرأ الأسئلة الشائعة حول ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [تعرف على كيفية ترحيل التطبيقات على أساس كل نظام أساسي.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)
3. إذا كانت لديك أسئلة إضافية بعد قراءة دليل النظام الأساسي للتطبيق، يمكنك النشر على [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) باستخدام العلامة [azure-ad-adal-deprecation] أو فتح مشكلة في مستودع GitHub الخاص بالمكتبة. راجع [القسم اللغات وأطر العمل من](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) مقالة نظرة **عامة حول MSAL** للحصول على ارتباطات إلى إعادة نشر كل مكتبة.
4. إذا كنت بحاجة إلى مساعدة في فهم التطبيقات التي تستخدم **ADAL،** فإننا ننصحك بمراجعة كل التعليمات البرمجية المصدر لتطبيقاتك. إذا كان ذلك قابلا للتطبيق، يمكنك التواصل مع أي موردي برامج مستقلة (ISVs) أو موفري التطبيقات. يمكن أن يوفر لك دعم Microsoft أيضًا قائمة بجميع تطبيقات ADAL غير التابعة لـ Microsoft في المستأجر الخاص بك.







