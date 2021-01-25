---
title: المشاكل المتعلقة بالارتباطات وعناوين Url
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
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974157"
---
# <a name="issues-with-links-and-urls"></a>المشاكل المتعلقة بالارتباطات وعناوين Url

أعاده توجيه عناوين Url للرد/الرد (يتم الآن لكل من التعبيرات) هي عناوين Url التي يستخدمها النظام الأساسي لهويه Microsoft لإرجاع الرموز المميزة المطلوبة للتطبيق. للحصول علي معلومات حول عناوين Url هذه ، راجع المقالات التالية:

- [تدفقات المصادقة وسيناريوهات التطبيقات](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) -معلومات حول معرفات uri لأعاده التوجيه في صفحه **تسجيل التطبيق** لكل سيناريو.
- [أعاده توجيه URI/قيود عنوان URL للرد والقيود](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**لا اعرف كيفيه تسجيل عنوان URL لأعاده توجيه URI/الرد لتطبيقي**

عندما تقوم بتسجيل الدخول باستخدام التطبيق الذي تقوم بتطويره ، إذا كان مربع الحوار تسجيل الدخول يعرض **AADSTS50011: لا يتطابق عنوان url الخاص بالرد <your app ID> المحدد في الطلب علي عناوين url للرد المكونة للتطبيق**، ستحتاج إلى اضافته إلى تسجيل التطبيقات ، وهو URI لأعاده التوجيه الذي استخدمته في التعليمات

لأضافه عنوان URL للرد ، انتقل إلى علامة التبويب **المصادقة** في صفحه **تسجيل التطبيق** في Azure portal وأضف إدخالا في القسم **أعاده توجيه URIs** . يتم كتابه معرفات Uri لأعاده التوجيه (ويب أو الهاتف المحمول/سطح المكتب). تعتمد القيمة التي يجب إدخالها علي نوع التطبيق الذي تقوم بإنشاءه ، كما هو موضح أدناه:

- بالنسبة إلى تطبيقات ويب أحاديه الصفحة ، فان عنوان URL للرد هو عنوان URL في التطبيق. راجع [تسجيل تطبيق الصفحة الواحد](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) أو [تسجيل تطبيق تطبيق ويب باستخدام مدخل Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- بالنسبة إلى تطبيقات سطح المكتب ، تعتمد القيمة التي يجب اختيارها علي:
    - النظام الأساسي (MacOS مختلف عن Windows أو Linux)
    - الطريقة التي تحصل فيها علي الرمز المميز (بطريقه تفاعليه ، باستخدام مصادقه Windows المتكاملة [إيفا] أو باستخدام username/password).
    للحصول علي التفاصيل ، راجع [تطبيقات سطح المكتب-تسجيل التطبيق-أعاده توجيه URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- بالنسبة لتطبيقات الاجهزه المحمولة ، تتوقف أعاده توجيه URI علي:
    - النظام الأساسي (iOS/Android/أوب)
    - ستساعدك المعلومات المستخدمة لإنشاء التطبيق ، مثل معرف الحزمة في نظام التشغيل iOS ، سيساعدك تسجيل الدخول وتجزئه التوقيع علي Android. للحصول علي التفاصيل ، راجع [تكوين النظام الأساسي وقم باعاده توجيه uri](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> واجات برمجه تطبيقات ويب وبعض الطرق الصامتة لجلب الرموز المميزة (إيفا واسم المستخدم/كلمه المرور) غير مطلوبه لأعاده توجيه URI.

**لقد قمت بنشر تطبيق ويب الخاص بي وعند اختبار التطبيق المنشور ، تظهر رسالة عدم تطابق عنوان url للرد**

أضف معرفات Uri لأعاده التوجيه لكل المواقع التي تقوم بنشر تطبيق ويب عليها. لمزيد من المعلومات ، راجع [تسجيل تطبيق web app باستخدام مدخل Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> أضف عنوان URI لأعاده التوجيه لموقع بعد نشر التطبيق في ذلك الموقع.

**تعذر تسجيل عناوين Url للردات كافيه**

أنت بائع البريد المستقل (ISV) ولديك معرفات واحده أو أكثر لأعاده توجيه البريد الخاصة بكل عميل لك. تريد الترحيل من ADAL/Azure AD v 1.0 إلى مسال/النظام الأساسي لهويه Microsoft وقد وصلت إلى [الحد الأقصى لعدد uri أعاده التوجيه](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). لحل هذه المشكلة ، [أضف التوجيه uri إلى أساسيات الخدمة](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) التي تتوافق مع كل عميل.
