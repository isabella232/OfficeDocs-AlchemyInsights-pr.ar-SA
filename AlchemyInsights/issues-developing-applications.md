---
title: مشاكل في تطوير التطبيقات
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013411"
---
# <a name="issues-developing-applications"></a>مشاكل في تطوير التطبيقات

لا استكشاف المشاكل الأكثر شيوعا وإصلاحها عند إنشاء تطبيقات Azure Active Directory (AD)، راجع المقالات التالية:

- [أواجه مشكلة في تسجيل الدخول إلى التطبيق (التطبيقات) باستخدام مستعرض Chrome فقط](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [لا أعرف كيفية تغيير الإعدادات الافتراضية لعمر الرمز المميز لتطبيقي](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [أشعر بالارتباك حول كيفية عمل موافقة التطبيق](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [لا أعرف كيفية منح الأذونات لتطبيقي](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [لا أفهم الفرق بين أذونات التطبيق والمفوضة](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***انتهاء الدعم لمكتبة مصادقة Azure Active Directory (ADAL) و Azure AD Graph API (AAD Graph)***

- اعتبارًا من 30 يونيو 2020، لن نضيف أي ميزات جديدة إلى مكتبة مصادقة Azure Active Directory (ADAL) وAPI لـ Azure AD Graph (AAD Graph). سنستمر في تقديم الدعم الفني وتحديثات الأمان ولكننا لن نقدم تحديثات للميزات بعد الآن.

- اعتبارًا من 30 يونيو 2022، سننهي دعم ADAL وAAD Graph، ولن نقدم بعد الآن دعمًا فنيًا أو تحديثات الأمان. نتيجة لهذا الشرط، فيما يلي النتائج المترتبة على ذلك:

    - ستستمر التطبيقات التي تستخدم ADAL على إصدارات نظام التشغيل الحالية في العمل بعد هذا الوقت ولكنها لن تحصل على أي دعم فني أو تحديثات الأمان.

    - قد لا تتلقى التطبيقات Graph AAD بعد هذا الوقت استجابات من نقطة Graph AAD

**ترحيل ADAL**

إذا كنت تستخدم تطبيقات Microsoft، نوصي بالتحديث إلى مكتبة مصادقة Microsoft (MSAL)، التي تحتوي على أحدث الميزات وتحديثات الأمان. هذه التوصية هي في سياق بدء Microsoft عملية تهجر تطبيقاتها إلى MSAL بحلول الموعد النهائي لنهاية الدعم. 

يضمن ترحيل Microsoft لتطبيقاتها إلى MSAL استفادة التطبيقات من تحسينات الميزات والأمان المستمرة ل MSAL.

1. [قراءة الأسئلة الشائعة حول ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [تعرّف على كيفية ترحيل التطبيقات على أساس كل نظام أساسي](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. إذا كنت بحاجة إلى مساعدة في فهم التطبيقات التي تستخدم ADAL، فإننا ننصحك بمراجعة التعليمات البرمجية المصدر لتطبيقاتك، وإذا كان ذلك قابلا للتطبيق، يمكنك التواصل مع أي موردي برامج مستقلين (ISVs) أو موفري التطبيقات. يمكن أن يوفر لك دعم Microsoft أيضًا قائمة بجميع تطبيقات ADAL غير التابعة لـ Microsoft في المستأجر الخاص بك.

**ترحيل AAD Graph**

بالنسبة للتطبيقات التي تستخدم AAD Graph، اتبع إرشاداتنا لترحيل تطبيقات AAD Graph إلى Microsoft Graph:

1. [توفر قائمة اختيار الترحيل نقطة بدء استخدام](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. يُُظهر مدخل تسجيل تطبيق Azure التطبيقات التي تستخدم AAD Graph. نوصي بمراجعة التعليمات البرمجية المصدر لتطبيقاتك، وإذا أمكن، التواصل مع أي موردي برامج مستقلين (ISVs) أو موفري تطبيقات مستقلين. يمكن أن يوفر لك دعم Microsoft أيضا معلومات Graph AAD للاستخدام في المستأجر.







