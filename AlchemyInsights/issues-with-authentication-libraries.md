---
title: مشاكل تتعلق بمكتبات المصادقة
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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063574"
---
# <a name="issues-with-authentication-libraries"></a>مشاكل تتعلق بمكتبات المصادقة

1. [تسرد مكتبات مصادقة](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) النظام الأساسي لهوية Microsoft مكتبات برامج وسطى ومدعمة من Microsoft ومتوافقة.
2. تدعم مكتبة مصادقة Microsoft (MSAL) العديد من تدفقات المصادقة [لاستخدامها](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) في سيناريوهات تطبيق مختلفة.
3. لمصادقة الرموز المميزة والحصول عليها، يمكنك تهيي تطبيق عميل عام أو سري جديد في التعليمات البرمجية. يمكنك تعيين عدة خيارات تكوين عند تهيئة تطبيق العميل في مكتبة مصادقة Microsoft (MSAL). لمعرفة المزيد، راجع [خيارات تكوين التطبيق.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**نهاية دعم Azure Active Directory Authentication Library (ADAL) و Azure AD Graph API (AAD Graph)**

**بدءا من 30 يونيو 2020،** لن نضيف أي ميزات جديدة إلى ADAL و Azure AD Graph. سنستمر في تقديم الدعم الفني وتحديثات الأمان ولكننا لن نقدم تحديثات للميزات بعد الآن.

**اعتبارا من 30 يونيو 2022،** سننهي دعم ADAL و Azure AD Graph ولن نوفر تحديثات الدعم التقني أو الأمان.

ستستمر التطبيقات التي تستخدم ADAL على إصدارات نظام التشغيل الموجودة في العمل بعد هذا الوقت ولكنها لن تحصل على أي تحديثات للدعم التقني *أو الأمان.*

قد لا تتلقى التطبيقات التي تستخدم Azure AD Graph بعد هذا الوقت استجابات من نقطة نهاية Azure AD Graph.

**ترحيل ADAL**

نوصي بالتحديث إلى [مكتبة مصادقة Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)، التي تحتوي على أحدث الميزات وتحديثات الأمان.

إذا كنت تستخدم تطبيقات Microsoft، فتعرف على أن Microsoft تقوم بتقليل تطبيقاتها إلى MSAL بحلول الموعد النهائي لنهاية الدعم، مع التأكد من أنها ستستفيد من تحسينات الميزات والأمان المستمرة في MSAL.

لمزيد من المعلومات، اطلع على:

1. [قراءة الأسئلة الشائعة حول ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [تعرّف على كيفية ترحيل التطبيقات على أساس كل نظام أساسي](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. إذا احتجت إلى مساعدة في فهم التطبيقات التي تستخدم ADAL، فإننا ننصحك بمراجعة كل التعليمات البرمجية المصدر للتطبيقات، وإذا كان ذلك قابلا للتطبيق، فصل إلى أي موفري خدمات الإنترنت أو موفري التطبيقات. يمكن أن يوفر لك دعم Microsoft أيضًا قائمة بجميع تطبيقات ADAL غير التابعة لـ Microsoft في المستأجر الخاص بك.

**ترحيل AAD Graph**

بالنسبة للتطبيقات التي تستخدم Azure AD Graph، اتبع الإرشادات الخاصة بترحيل تطبيقات [Azure AD Graph إلى Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [توفر قائمة اختيار الترحيل نقطة بدء.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. يُُظهر مدخل تسجيل تطبيق Azure التطبيقات التي تستخدم AAD Graph. نوصيك بمراجعة جميع التعليمات البرمجية المصدر لتطبيقاتك، وإذا أمكن، يمكنك الوصول إلى أي من موردي البرامج المستقلين أو مزودي التطبيقات. يمكن أن يوفر لك دعم Microsoft أيضا قائمة بجميع استخدام AAD Graph في المستأجر الخاص بك.
3. لكي يمكن لتطبيقك الوصول إلى البيانات في Microsoft Graph، يجب على المستخدم أو المسؤول منحه الأذونات الصحيحة عبر عملية موافقة. يسرد [مرجع أذونات Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) الأذونات المقترنة بكل مجموعة رئيسية من واجهات برمجة تطبيقات Microsoft Graph. كما يوفر إرشادات حول كيفية استخدام الأذونات.
