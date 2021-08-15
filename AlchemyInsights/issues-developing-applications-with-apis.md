---
title: مشاكل في تطوير التطبيقات باستخدام واجهات برمجة التطبيقات
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
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013447"
---
# <a name="issues-developing-applications-with-apis"></a>مشاكل في تطوير التطبيقات باستخدام واجهات برمجة التطبيقات

لبدء استخدام Azure Active Directory Graph API، راجع دليل البدء السريع ل [Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ، أو عرض وثائق مرجع [Azure AD Graph API التفاعلية](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**انتهاء الدعم لمكتبة مصادقة Azure Active Directory (ADAL) و Azure AD Graph API (AAD Graph)**

**بدءا من 30 يونيو 2020،** لن نضيف أي ميزات جديدة إلى ADAL و Azure AD Graph. سنستمر في تقديم الدعم الفني وتحديثات الأمان ولكننا لن نقدم تحديثات للميزات بعد الآن.

**بدءا من 30 يونيو 2022،** سننهي دعم ADAL و Azure AD Graph ولن نوفر تحديثات الأمان أو الدعم التقني.

ستستمر التطبيقات التي تستخدم ADAL على إصدارات نظام التشغيل الحالية في العمل بعد هذا الوقت ولكنها لن تحصل على أي دعم فني أو تحديثات الأمان.

قد لا تتلقى التطبيقات التي تستخدم Azure AD Graph بعد هذا الوقت استجابات من نقطة نهاية Azure AD Graph نهاية.

**ترحيل ADAL**

نوصي بالتحديث إلى [مكتبة مصادقة Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)، التي تحتوي على أحدث الميزات وتحديثات الأمان.

إذا كنت تستخدم تطبيقات Microsoft، فتعرف على أن Microsoft تقوم بتهجر تطبيقاتها إلى MSAL بحلول الموعد النهائي لنهاية الدعم، مع التأكد من أنها ستستفيد من تحسينات الميزات والأمان المستمرة ل MSAL.

1. [اقرأ الأسئلة الشائعة حول ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [تعرف على كيفية ترحيل التطبيقات على أساس كل نظام أساسي.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. إذا كنت بحاجة إلى مساعدة في فهم التطبيقات التي تستخدم ADAL، فإننا ننصحك بمراجعة التعليمات البرمجية المصدر لتطبيقاتك، وإذا كان ذلك قابلا للتطبيق، فصل إلى أي موفري خدمات الإنترنت أو موفري التطبيقات. يمكن أن يوفر لك دعم Microsoft أيضًا قائمة بجميع تطبيقات ADAL غير التابعة لـ Microsoft في المستأجر الخاص بك.

**ترحيل AAD Graph**

بالنسبة للتطبيقات التي تستخدم Azure AD Graph، اتبع إرشاداتنا لترحيل [تطبيقات Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)إلى Microsoft Graph .

1. [توفر قائمة اختيار الترحيل نقطة بدء استخدام](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. يُُظهر مدخل تسجيل تطبيق Azure التطبيقات التي تستخدم AAD Graph. نوصيك بمراجعة جميع التعليمات البرمجية المصدر لتطبيقاتك، وإذا أمكن، يمكنك الوصول إلى أي من موردي البرامج المستقلين أو مزودي التطبيقات. يمكن أن يوفر لك دعم Microsoft أيضا قائمة بكل برامج AAD Graph في المستأجر.
1. لكي يمكن لتطبيقك الوصول إلى البيانات في Microsoft Graph، يجب على المستخدم أو المسؤول منحه الأذونات الصحيحة عبر عملية موافقة. يسرد [مرجع Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) Microsoft الأذونات المقترنة بكل مجموعة رئيسية من واجهات برمجة التطبيقات Graph Microsoft. كما يوفر إرشادات حول كيفية استخدام الأذونات.
