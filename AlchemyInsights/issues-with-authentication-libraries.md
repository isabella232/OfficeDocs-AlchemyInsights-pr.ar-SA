---
title: المشاكل المتعلقة بمكتبات المصادقة
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54027991"
---
# <a name="issues-with-authentication-libraries"></a>المشاكل المتعلقة بمكتبات المصادقة

1. [النظام الأساسي للهويات في Microsoft مكتبات المصادقة على](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) مكتبات البرامج المتوسطة والعميل المعتمدة من Microsoft والمتوافقة.
2. تدعم مكتبة مصادقة Microsoft (MSAL) العديد من تدفقات المصادقة [لاستخدامها](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) في سيناريوهات تطبيق مختلفة.
3. لمصادقة الرموز المميزة والحصول عليها، يجب تهيييه تطبيق عميل عام أو سري جديد في التعليمات البرمجية الخاصة بك. يمكنك تعيين عدة خيارات تكوين عند تهيئة تطبيق العميل في مكتبة مصادقة Microsoft (MSAL). لمعرفة المزيد، راجع [خيارات تكوين التطبيق](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**انتهاء الدعم لمكتبة مصادقة Azure Active Directory (ADAL) و Azure AD Graph API (AAD Graph)**

**بدءا من 30 يونيو 2020،** لن نضيف أي ميزات جديدة إلى ADAL و Azure AD Graph. سنستمر في تقديم الدعم الفني وتحديثات الأمان ولكننا لن نقدم تحديثات للميزات بعد الآن.

**بدءا من 30 يونيو 2022،** سننهي دعم ADAL و Azure AD Graph ولن نوفر تحديثات الأمان أو الدعم التقني.

ستستمر التطبيقات التي تستخدم ADAL على إصدارات نظام التشغيل الموجودة في العمل بعد هذا الوقت ولكنها لن تحصل على أي تحديثات أمنية أو *دعم تقني.*

قد لا تتلقى التطبيقات التي تستخدم Azure AD Graph بعد هذا الوقت استجابات من نقطة نهاية Azure AD Graph نهاية.

**ترحيل ADAL**

نوصي بالتحديث إلى [مكتبة مصادقة Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)، التي تحتوي على أحدث الميزات وتحديثات الأمان.

إذا كنت تستخدم تطبيقات Microsoft، فتعرف على أن Microsoft تقوم بتهجر تطبيقاتها إلى MSAL بحلول الموعد النهائي لنهاية الدعم، مع التأكد من أنها ستستفيد من تحسينات الميزات والأمان المستمرة ل MSAL.

لمزيد من المعلومات، اطلع على:

1. [قراءة الأسئلة الشائعة حول ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [تعرّف على كيفية ترحيل التطبيقات على أساس كل نظام أساسي](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. إذا كنت بحاجة إلى مساعدة في فهم التطبيقات التي تستخدم ADAL، فإننا ننصحك بمراجعة التعليمات البرمجية المصدر لتطبيقاتك، وإذا كان ذلك قابلا للتطبيق، فصل إلى أي موفري خدمات الإنترنت أو موفري التطبيقات. يمكن أن يوفر لك دعم Microsoft أيضًا قائمة بجميع تطبيقات ADAL غير التابعة لـ Microsoft في المستأجر الخاص بك.

**ترحيل AAD Graph**

بالنسبة للتطبيقات التي تستخدم Azure AD Graph، اتبع إرشاداتنا لترحيل [تطبيقات Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)إلى Microsoft Graph .

1. [توفر قائمة اختيار الترحيل نقطة بدء.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. يُُظهر مدخل تسجيل تطبيق Azure التطبيقات التي تستخدم AAD Graph. نوصيك بمراجعة جميع التعليمات البرمجية المصدر لتطبيقاتك، وإذا أمكن، يمكنك الوصول إلى أي من موردي البرامج المستقلين أو مزودي التطبيقات. يمكن أن يوفر لك دعم Microsoft أيضا قائمة بكل برامج AAD Graph في المستأجر.
3. لكي يمكن لتطبيقك الوصول إلى البيانات في Microsoft Graph، يجب على المستخدم أو المسؤول منحه الأذونات الصحيحة عبر عملية موافقة. يسرد [مرجع Graph](https://docs.microsoft.com/graph/permissions-reference) Microsoft الأذونات المقترنة بكل مجموعة رئيسية من واجهات برمجة التطبيقات Graph Microsoft. كما يوفر إرشادات حول كيفية استخدام الأذونات.
