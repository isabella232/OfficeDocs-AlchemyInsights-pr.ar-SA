---
title: المشكلات المتعلقة بالارتباطات وعناوين URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 1387d7e0cdf2e730b2812f3970181d2bf889d44b1faab9a351911840909defb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054785"
---
# <a name="issues-with-links-and-urls"></a>المشكلات المتعلقة بالارتباطات وعناوين URL

عنوان URL لإعادة التوجيه، أو عناوين URL للردود (وكلا التعبيرين مرادف للآخر)، هي عناوين URL التي يستخدمها النظام الأساسي للهويات في Microsoft في إرجاع الرموز المميزة التي يطلبها التطبيق. للاطلاع على معلومات حول عناوين URL هذه، راجع المقالات التالية:

- [عمليات تدفق المصادقة وسيناريوهات التطبيق](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - معلومات حول عناوين URL لإعادة التوجيه في صفحة **تسجيل التطبيق** لكل سيناريو.
- [القيود والحدود لعنوان URL لإعادة التوجيه أو عناوين URL للردود](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**لا أعرف كيفية تسجيل عنوان URL الصحيح لإعادة التوجيه، أو عناوين URL للردود، من أجل التطبيق**

عندما تسجّل الدخول باستخدام التطبيق الذي تعمل على تطويره، إذا تم عرض مربع حوار تسجيل الدخول الرسالة التالية **AADSTS50011: عنوان URL للرد المحدد في الطلب لا يطابق عناوين URL للردود التي تم تكوينها للتطبيق <your app ID>**، فسوف يلزمك أن تضيف إلى تسجيل التطبيق عنوان URL لإعادة التوجيه والذي استخدمته تعليماتك البرمجية في طلب الرمز المميز المُقدَّم إلى النظام الأساسي للهويات في Microsoft.

لإضافة عنوان URL للردود، انتقل إلى علامة تبويب **مصادقة** في صفحة **تسجيل التطبيق** لديك في مدخل Azure، وأضِف إدخالاَ في المقطع **عناوين URL لإعادة التوجيه**. تعتمد القيمة التي يلزم إدخالها على نوع التطبيق الذي تنشئه، كما هو موضح أدناه:

- بالنسبة للتطبيقات وتطبيقات الويب ذات الصفحة الواحدة، يكون عنوان URL للرد هو عنوان URL في تطبيقك. راجع [تسجيل تطبيق من صفحة واحدة](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) أو [تسجيل تطبيق ويب باستخدام مدخل Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- بالنسبة لتطبيقات سطح المكتب، تعتمد القيمة التي يلزم اختيارها على:
    - النظام الأساسي (يختلف نظام MacOS عن Windows أو Linux)
    - طريقة الحصول على الرمز المميز (بشكل تفاعلي، أو باستخدام تدفق رموز الجهاز، أو باستخدام مصادقة Windows المتكاملة [IWA]، أو باستخدام اسم المستخدم/كلمة المرور).
    للاطلاع على التفاصيل، راجع [تطبيقات سطح المكتب - تسجيل التطبيق - عناوين URL لإعادة التوجيه](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- بالنسبة لتطبيقات الأجهزة المحمولة، تعتمد عناوين URL لإعادة التوجيه على:
    - النظام الأساسي (iOS/Android/UWP)
    - المعلومات المُستخدمة في إنشاء التطبيق، مثل معرّف المجموعة في نظام التشغيل iOS واسم الحزمة وتجزئة التوقيع، تساعدك في تسجيل تطبيق مدخل Azure على نظام التشغيل Android. للاطلاع على التفاصيل، راجع [تكوين النظام الأساسي وعناوين URL لإعادة التوجيه](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> واجهات برمجة تطبيقات الويب وبعض الطرق التلقائية للحصول على الرموز المميزة (مصادقة Windows المتكاملة واسم المستخدم/كلمة المرور) إلا تتطلب عنوان URL لإعادة التوجيه.

**لقد نشرت تطبيق الويب الخاص بي، وعند اختبار التطبيق المنشور أجد رسالة تفيد بعدم تطابق عنوان URL للردود**

يمكنك إضافة عناوين URL لإعادة التوجيه لكل المواقع التي تنشر فيها تطبيق الويب الخاص بك. للحصول على مزيد من المعلومات، راجع [تسجيل تطبيق ويب باستخدام مدخل Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> يمكنك إضافة عناوين URL لإعادة التوجيه لأحد المواقع مباشرةً بعد نشر التطبيق في ذلك الموقع.

**لا يمكنني تسجيل عدد كافٍ من عناوين URL للردود**

أنت مورد برامج مستقل ولديك واحد أو أكثر من عناوين URL لإعادة التوجيه لكل عميل لديك. أنت تريد الترحيل من ADAL/Azure AD v1.0 إلى MSAL/النظام الأساسي للهويات في Microsoft، ووصلت إلى [أقصى عدد من عناوين URL لإعادة التوجيه](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). لحل هذه المشكلة، [أضِف عناوين URL لإعادة التوجيه إلى أساسيات الخدمة](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) التي تتوافق مع كل عميل من عملائك.
